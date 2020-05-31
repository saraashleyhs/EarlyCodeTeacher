{% include "../includes/header.md" %}

# CSS Selectors

*****

**Objective:** By the end of this lesson, the student will apply styles by targeting HTML elements based their relationships with one another.

**Assignment:**
CSS Diner
CSS Selectors Practice (Part 1)

*****

#### Review and Recap

Previously, we have covered how to write CSS rules to add some style to our webpage.
Remind yourself of the 3 parts of a CSS rule:

 <img style="margin:auto; width:200px" src="../images/css-rule-anatomy.jpg">

 We will focus on the selector piece of the rule.  Before today, we have only used the tag-type selector. 
 #### Type Selectors

The `type selector` simply selects any element specified by its type. Unless you modify it with additional selections, a type selector will affect every instance of that type. If you write one `a` selector, you would then change the styling for every `a` element within the page. Because of this, type selectors are usually reserved for doing just that:

`index.html`
```html
<div>This is a basic section element.</div>
```

`css/style.css`
```css
div {
  text-align: center; 
}
``` 


*****

## Element Relationships

Writing HTML creates structure for our webpage.  Remember, the opening and closing tags create a container to hold content.  There are plenty of times where our container can also hold *other elements*.  This creates a relationship between the outside element and inside element.  See the example below:

```html
<body>
    <main>
        <p></p>
        <div></div>
    </main>
</body>
```
The **body** element is the direct parent of the **main** element.  The **p** element and **div** element are direct children of the **main** element. 
Notice that the **p** element and **div** element are both contained within the **main** element. They are considered sibling elements.  

* You can target elements based its relationship with other elements.  

*****

## Class Selector 

Take a look at the HTML code block below.

```html
<div>This is the first element</div>
<p>This is the second element</p>
<p>This is the third element</p>
```

How can I target(select) and apply different styles to each of the paragraph elements?

* If I choose to use the tag selector (p) then it will apply the styles to all of the p elements.

I can fix my problem by assigning a class to each of the HTML elements.  Choose a class name that relates to what you are selecting or trying to do with element.

```html
<div class ="first">This is the first element</div>
<p class ="second">This is the second element</p>
<p class ="third">This is the third element</p>
```

To use each class name in the CSS, it would look like:

```css
.first{
    color: #32a0a8;
    text-align: left;
}

.second{
    color: #99295a;
    text-align: center;
}

.third{
    color: rgb(96, 40, 148);
    text-align: right;
}
```

* Notice the (.) in front of the class name.  

#### Reusing Class Selectors

If you want to give multiple elements the same styles, this can also be achieved by using Classes.

**HTML:**
```HTML

<div class="same-elements">The first and second paragraph elements will have the same style</div>
<!-- more html -->
<p class="same-elements">Because they were given the same class.</p>
<!-- more html -->
<p class="different-element">This is the third paragraph element</p>
```

**CSS:**

```css
.same-elements{
    color: #32a0a8;
    text-align: left;
}

.different-element{
    color: rgb(96, 40, 148);
    text-align: right;
}
```

Copy and paste the code from this section out in a [CodePen](https://codepen.io/pen/) to investigate. You dont have to save this practice.

*****

## Id Selector

Take a look at the HTML code block below.

```html
<p>This is the first paragraph element</p>
<p>This is the second paragraph element</p>
<p>This is the third paragraph element</p>
```

Using the same HTML above, we could give each element a **UNIQUE** Id.

* An ID has to be unique! This means that you cannot reuse the same id in the same HTML document.

I can assign CSS styles to each .

```html
<p id ="first">This is the first paragraph element</p>
<p id ="second">This is the second paragraph element</p>
<p id ="third">This is the third paragraph element</p>
```

To use each ID in the CSS, it would look like:

```css
#first{
    color: #32a0a8;
    text-align: left;
}

#second{
    color: #99295a;
    text-align: center;
}

#third{
    color: rgb(96, 40, 148);
    text-align: right;
}
```

* Notice the (#) in front of the class name.  

##### An id cannot be reused, so it should be used when you want to give unique styles to an element.

Copy and paste the code from this section out in a [CodePen](https://codepen.io/pen/) to investigate. You dont have to save this practice.

*****

> To remember the syntax for CSS Id and class:
> * Class - think of classes in school.  Class Periods (.class-name)
> * Id - each student has a unique Id number (#id-name)

*****

## Practice It - [CSS Diner](https://flukeout.github.io/#)

1. Go through each level to select the correct piece in the diner.  

1. You will get practice on a variety of selectors.  Use the hints in the right-hand panel.

    > If you don't know how to do something right away, remember S.A.T.!!  Search for the answer in your textbook or Google, Ask your classmates and/or teacher, then Teach your solution. Another student may have the same question.

1. CSS Diner
    <iframe
     src="https://flukeout.github.io/#"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="CSS Diner"
     >
     </iframe>

   <br>

*****

## Assignment- [Selectors Practice Part 1](https://codesandbox.io/s/selectors-practice-05e4o?fontsize=14&hidenavigation=1&theme=dark)

* Your assignment is to complete the CSS file. You will not change the HTML.  Have a go at those bonus challenges too!
<br>

    >  NOTE:  You will return to this assignment when completing the Pseudo-Classes Lesson.

<iframe
     src="https://codesandbox.io/embed/selectors-practice-05e4o?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Selectors Practice"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

*****

### Know Your Docs

Be sure to reference the official documentation on [CSS Selectors](https://www.w3schools.com/cssref/css_selectors.asp) from W3Schools. Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******

## Questions for Class Discussion

1. What is a selector?
1. Name 5 different element relationships and how you would select them in your CSS.  
1. How do you use a class selector?  
1. How would you use an id selector?  
1. What problem would you be trying to solve when you use a class? an ID?

*****

### Terminology to Know

Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

* Class Selector
* Id Selector
* Parent Element
* Selector

*****
<!--TODO Include the Cascade-->

### Let's go to the next Lesson [Pics, Vids, and Links >](MediaTags.md)

{% include "../includes/footer.md" %}
