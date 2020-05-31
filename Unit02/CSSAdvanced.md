{% include "../includes/header.md" %}

# Advanced CSS Techniques

*****

**Objective:** By the end of this lesson, the student will use W3Schools as a resource to apply additional styles to HTML elements using CSS rules.

**Assignment:** CSS Advanced Practice CodeSandbox

*****

#### Review and Recap

Previously, we covered how to write CSS rules to add some style to our webpage.
Remind yourself of the 3 parts of a CSS rule:

 <img style="margin:auto; width:500px" src="../images/css-rule-anatomy.jpg">


* For today's activity, we will explore CSS a little deeper into the different properties that we could change about an object.  You will use [W3Schools](https://www.w3schools.com/css/default.asp) to help you complete the assignment.

<br>

 > Hint: You may have to use previous lesson material to help you.  Use your resources to complete the assignments.

*****

## Targeting multiple selectors

If you want to apply the same style to multiple HTML elements, using a comma (,) will allow this to happen.

```css
Applying color values to both the an h3 and p tags:

h3 , p {
    color: blue;
    font-family: Arial, Helvetica, san-serif;
}

```

This will make all the h3 headers and the paragraph elements blue and change the font to Helvetica.  

*****

## Color Codes

There are different ways to assign a color value to an element.  

Three of those color models are:

* By Color Name
    * You can use the names of some colors.
    * This option limits the choice that you have for colors because the color has to have a Name.

    ```css 
    color: blue; 
    ```
**For all other shades that don't necessaraily have names, we use a code:**
* By Hex Code
    * Hex code is a code represented by combination of letters and numbers.

    ```css 
    color: #0000ff; 
    ```

* By Red, Green, Blue values (called RGB values)
    * All colors on a computer are different combinations of values of red, green, and blue.

    ```css 
    color: rgb(0, 0, 255); 
    ```

**<p style="font-size:18px;">All of these codes are for the exact same color!</p>**

There are tools like this [Color Picker](https://www.google.com/search?q=color+picker) that can help you choose a color and it will give you the code!

Another great tool is the [Adobe Color Wheel](https://color.adobe.com/create/color-wheel) where you can create a custom color scheme for any project.  

*****

## Practice It - Advanced Practice [CodeSandbox](https://codesandbox.io/s/css-advanced-practice-inw3y?fontsize=14&hidenavigation=1&theme=dark)

1. Fork the following CodeSandbox.
    <iframe
     src="https://codesandbox.io/embed/css-advanced-practice-inw3y?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="CSS Advanced Practice"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

   <br>

1. You will have to create and link your CSS stylesheet. *(Hint: Use your resources to remind yourself how to do this)*

1. Follow the instructions in the CodeSandbox to style the HTML elements.

> If you don't know how to do something right away, remember S.A.T.!!  Search for the answer in your textbook or Google, Ask your classmates and/or teacher, then Teach your solution. Another student may have the same question.

*****

### Know Your Docs

Be sure to reference the official documentation on [CSS on W3Schools](https://www.w3schools.com/css/default.asp) Tutorials. Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******

## Questions for Class Discussion

1. What is a selector?
1. What are the different ways to assign a color value to an element?  
1. How do you make sure that the HTML file and CSS file are linked together?
1. Can you change more than one property in a declaration block?

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
<!--TODO Include the Cascade-->

### Let's go to the next Lesson [Selectors >](Selectors.md)

{% include "../includes/footer.md" %}
