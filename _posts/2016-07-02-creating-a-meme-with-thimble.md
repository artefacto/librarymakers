---
layout: post
title: Create your own meme with Thimble
categories: [recipes]
tags: [thimble, coding, images, html, webmakers]
---

## Intro
Thimble is part of the Mozilla webmaker tools designed to help learn and teach coding in HTML and CSS.

You can create your own web pages or remix existing web pages and publish them online.
This example will walk you through creating and sharing your own meme image by creating a simple HTML page and styling it using CSS.

What we want to create is something like this:

![Example meme]({{ base.url }}/assets/img/blog/thimble/example-meme.png)


## What you need

- Thimble is feely available to use via https://thimble.mozilla.org/. To save and publish your work, you'll need to create an account.
- A meme image - To find public domain images to use for your meme, try the [Public Domain Archive](http://publicdomainarchive.com/) or [Pixabay](pixabay.com).


## How

Start a new project with Thimble at: [https://thimble.mozilla.org/](https://thimble.mozilla.org/)

Click on ‘Start a project from scratch'

What we want to create is something with an image and 2 captions (as above).

When we start, we have the Thimble default page that includes a heading and a paragraph. The headings are assigned number levels so for a large header you use `<h1>` tags and for smaller headers you can use `<h6>`. HTML tags need to be opened and closed. So for our first header, we can change it to be:

`<h1>First caption goes here</h1>`

We won’t be using the paragraph for this project, so you can delete the `<p>…</p>` section.

You can update the title for your project too. Your project should now look something like this:

    <!DOCTYPE html>
    <html>
    <head>
     <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>My Meme</title>
     <link rel="stylesheet" href="style.css">
    </head>
    <body>
      <h1>First caption goes here</h1>
    </body>
    </html>

Now we need to add an image.

Add an image. you can upload new files using the file upload button on the left.


![Upload an image]({{ base.url }}/assets/img/blog/thimble/Thimble-upload-file_annotated.png)

Your uploaded image should now appear in the file list (alongside the CSS and index.html file)

Under the `<h1>` tags, add an image tag that includes your image file name,  like this:

    <img src="cat-image.jpeg" />

 Images are a bit different to other tags in that they don’t have open and closing tags, but have a self-closed `/>` at the end.

You can also set a width attribute for the image

    <img src="cat-image.jpeg” width=700 />

You can now also add a second heading underneath the image. this time we will make it a second-level heading, using the *h2* tag.

    <h2> My second heading</h2>

The html page should now look like this:

    <!DOCTYPE html>
    <html>
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1">
      <title>My Meme</title>
      <link rel="stylesheet" href="style.css">
    </head>
    <body>

      <h1>First caption goes here</h1>

      <img src="cat-image.jpeg" />

      <h2> My second heading</h2>

    </body>
    </html>


But it doesn’t yet look quite right. To change how the page looks, we need to edit the CSS file. Cascading Style Sheets (CSS) allow you to change the appearance of your HTML elements. Click on `style.css` from the file menu to edit the stylesheet.

Here, you can see the style attributes for the body of the page. We can also add styles to different elements like the headings and images.

It's quite common for the text on meme images to be all in capitals, so we can set our headings to be in uppercase and also change the colours of the page.

If you use a particular style more than once, you can use it as a class. for example if we give both the headings a class of ‘capitalise’ in the html file:

e.g. `<h1 class="capitalise">Heading 1 goes here</h1>`

We can then reference that in the stylesheet using a dot followed by the class name.

Update your stylesheet to look like this:

    body {
      font-family: "Open Sans", sans-serif;
      background: #111111;
      color: #ffffff;
      }

    .capitalise {
     text-transform: uppercase;
      }

    h1 {
      text-align: center;
      }

    h2 {
       margin-top: -2em;
       text-align: center;
      }

    img {
       width: 750px;
       height: auto;
       }

Now, you can edit the text for your meme and make any additional changes to the styles that you want.

![Demo meme]({{ base.url }}/assets/img/blog/thimble/meme-example-complete.png)

(something like this except funnier)

Once your meme is ready, click publish to share it with the world.


![Publish your meme]({{ base.url }}/assets/img/blog/thimble/publish-your-project.png)

### Credits
Partly inspired by the original Webmaker project by Laura Fleming ([now archived](https://thimble.webmaker.org/project/60766/remix))
