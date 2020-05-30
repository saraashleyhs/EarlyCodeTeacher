{% include "../includes/header.md" %}

# Intro to HTML

*****

**Objective:** By the end of this lesson, the student will be able to identify meaningful HTML tags and elements.

**Assignment:** Meaningful Tags CodeSandbox

*****

## Before we code

We need to get to know some characters on our keyboard before we can code. Use the presentation below to learn about these characters and what we use them for.

<iframe style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;" src="https://docs.google.com/presentation/d/e/2PACX-1vQcmAwU6zCSjkBbb93aLNKs6zxPKd04oxPEPPWW0vJZnt2jTN3tumToUv4hDmoSi5irCT_ei2rb9ywz/embed?start=false&loop=false&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

### Play your way to understanding
#### -Play the quizlet game to show your mastery of your keyboard characters.

<iframe src="https://quizlet.com/470157445/match/embed?x=1jj1" height="500" width="100%" style="border:0"></iframe>

*****

## What is Hyper-Text Markup Language(HTML)?

HTML is the standard mark-up language for creating Web Pages.  The following are the main points about HTML:

- HTML stands for HyperText Markup Language
- HTML describes the structure of a Web page
- An HTML document consists of a series of elements
- HTML elements tell the browser how to display the content
- HTML elements are represented by tags
- HTML tags label pieces of content such as “header”, “paragraph”, “list”, and so on
- Browsers do not display the HTML tags, but use them to render the content of the page

A basic HTML template looks like the following:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Static Template</title>
  </head>
  <body>
    <h1>This is a basic static template!</h1>
  </body>
</html>
```
##### What do you notice? What do you wonder?
*****

## HTML Structure

  ### Tags

  ```html
  <h1> </h1>
  The <h1> is an opening tag for a header1 element.
  The </h1> is a closing tag for a header1 element.

  What is the difference between the two?


  All of the content displayed on the webpage is between the two 
  <body> </body> tags.
  ```

   The opening and closing tags create the container that will hold the content.  Think of the closing tag as the **lid** on the container.
   <br>
  <img width=400px src="../images/tags.jpg">


  ### Elements
  When we place content between the two tags, we have created an HTML **element**.
  ```html
  <h1>Content between the opening and closing tag.</h1>

  The whole thing represents an H1 element.
  There are lots of other types of elements depending on the tag that is used.
  They each represent different objects that the browser sees.
  
  ```

  Explore the different types of elements before moving on to the practice activity.
  
  [HTML Tags Reference](https://www.w3schools.com/TAGS/default.ASP)

******

## Meaningful Elements

We are now going to practice using different tags to create some structure to an HTML document.  Follow the instructions in the code comments to use the correct tags.

#### Project Directions:

1. Open the CodeSandbox below
1. Make sure you are signed in.
1. Fork your own copy.
1. Follow the directions in the comments to complete the assignment.

<iframe
     src="https://codesandbox.io/embed/meaningful-tags-practice-q4yus?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Meaningful tags Practice"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts allow-autoplay"
   ></iframe>

  ```html
  Hint: A comment in the code is indicated by the following syntax.

 <!--This is an HTML comment -->

 Does a comment show up in the browser?
  ```

******

### Questions for Class Discussion

1. What does HTML stand for?
1. What is the difference between an HTML tag and HTML element?
1. Does the content in the ```<head></head>```element appear on the webpage?
1. How do you comment code out so that the browser doesn't display it?
1. Why is it important to use meaningful tags?
1. Does it matter the way we code our elements into the HTML file? (What would happen if you left off the closing tag?)

*****

### Terminology to Know
<!-- @TODO ATTENTION: DEVELOPER, In this section, we list terms students should now and be able to discuss at this point. Be sure to list a few for the students to jot down and work with. -->
Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

- HTML
- Browser
- Opening Tag
- Closing Tag
- Element
- Tag
- Comment
- Carat

*****

## Let's get ready for next lesson [CSS Intro >](CSS-Intro.md)

{% include "../includes/footer.md" %}
