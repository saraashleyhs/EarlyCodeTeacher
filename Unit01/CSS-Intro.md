{% include "../includes/header.md" %}

# Intro to CSS

*****

**Objective:** By the end of this lesson, the student will be able to apply styles to HTML elements using CSS rules.

**Assignment:** CSS Practice CodeSandbox

*****

#### Review and Recap

In the last lesson, we covered how to use HTML tags to add structure to our webpage.
All HTML elements have properties that can be given different values. When we do this, it will change how those elements are styled on the page. We will explore that using CSS.
*****

## What is CSS?

CSS stands for Cascading Style Sheets. CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

Using CSS allows us change properties attached to HTML elements.  You saw in the previous assignment that some HTML elements looked differently.  


For example: 
<div style="border:2px solid black; padding-bottom:5%">
<h1 style="text-align: center">An H1 heading</h1>
<h3 style="text-align: center">An H3 heading</h3>
</div>
<br>

These two elements have properties, such as the  *font size*, that start out with different default values. In our CSS file, we can change lots of different properties.

*****

#### Read It - Properties

A property is an attribute that an element has access to. We can change the value of any property that CSS has available.  Go to [W3Schools](https://www.w3schools.com/cssref/default.asp) and look through the properties.  These are all of the different attributes that you can change about an HTML element.

*****

### Where does CSS go?

There are different ways to apply CSS to the HTML.  We are going to focus on the ***external*** method.  This means the CSS styles will be contained in a separate file. The HTML and CSS will be in separate files and so we have to make sure the HTML and CSS files are **linked together**.

```html
Link your CSS file by copying and pasting the following code
into the <head></head> of your HTML:

<link rel="stylesheet" href="style.css">


"style.css" is the name of the file that contains your CSS styles.
The file name could be different, but it has to have the .css on the end.
```

*****
*****

## What does CSS look like?

Now that we know what CSS is, let's take a look at how it is written.

#### CSS Syntax 
A *CSS rule* consists of a **selector** and a **declaration** block.

<p><img src="../images/CodeSandbox/img_selector.gif" alt="CSS selector" class="w3-image"></p>

* The selector points to the HTML element to style; here it's the h1. (The thing from our HTML that gets the styles attached to it).

* The declaration block (in curly braces) contains one or more declarations separated by semicolons. Each declaration changes a different property.

* Each declaration includes a CSS property name and a value, separated by a colon.

* Separate declarations with a semicolon.

* In the above example, there are two declarations being made on the selected h1 element:
  * The color property is being given a value of blue.
  * The font-size property is being given a value of 12 pixels.

******


### Practice It - [CodeSandbox](https://codesandbox.io/s/css-practice-k79ks?fontsize=14&hidenavigation=*theme=dark)

Fork the embedded CodeSandbox to practice adding styles to HTML Elements.

The rule templates are already in the CSS file. Fill in the correct properties and values to complete each task.  

You will need match the HTML elements with their CSS declaration.  

<iframe
     src="https://codesandbox.io/embed/css-practice-k79ks?fontsize=14&hidenavigation=*theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="CSS Practice"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts allow-autoplay"
   ></iframe>


[![Edit CSS Practice](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/css-practice-k79ks?fontsize=14&hidenavigation=*theme=dark)

******

### TL - DR
Watch this video for a mini-crash course in CSS.

<iframe width="560" height="315" src="https://www.youtube.com/embed/3T4BsrBISnI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Know Your Docs 

Be sure to reference the official documentation on [CSS on W3Schools](https://www.w3schools.com/css/default.asp) Tutorials. Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******

## Questions for Class Discussion

* What does CSS do?
* What is a selector?
* What is a declaration block?
* How do you make sure that the HTML file and CSS file are linked together?
* Can you change more than one property in a declaration block?

*****

### Terminology to Know

Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

* CSS
* Declaration
* Selector
* Link
* Property
* Value

*****


### Let's go to the next Lesson [Wireframing >](Wireframing.md)

{% include "../includes/footer.md" %}
