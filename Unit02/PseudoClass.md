{% include "../includes/header.md" %}

# Pseudo-Class Selectors

*****

**Objective:** By the end of this lesson, the student will give HTML elements dynamic styles using Psuedo-classes.

**Assignment:** CSS Selectors Practice (Part 2)

*****

### Overview

Take a moment to think about one of your favorite websites that you visit.  Are there effects that happen when you open the page or when you hover over certain objects?  These can be coded using a special CSS component.  

We can add those dynamic elements to our webpages too using Pseudo-Classes!!!

*****

## Pseudo Selectors

#### Pseudo-class selectors

A CSS pseudo-class is a keyword added to selectors that specifies a special *characteristic* or *state* of the element we are targeting.

For example, `:hover` will apply a style when the user's mouse hovers over the element specified by the selector. These special state attributes won't be written in the HTML, but are ready to be manipulated using CSS.

  `css/style.css`

```css
  selector:pseudo-class {
    property: value;
  }
```

Explore the different Psuedo-classes on [W3Schools Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp).

#### Practice it - Pseudo Classes

The CodeSandbox below has some Psuedo Classes applied to some of the HTML elements.  
After you have had some time to explore what you think each are doing, **discuss** your ideas as a class.  

* Fork a copy of the [CodeSandbox](https://codesandbox.io/s/pseudo-classes-7yg52?fontsize=14&hidenavigation=1&theme=dark)
* Follow the instructions in the CodeSandbox below.
<iframe
     src="https://codesandbox.io/embed/pseudo-classes-7yg52?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Pseudo-Classes"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

*****

## Practice It - CSS Selectors Practice

1. Go to your CSS Selectors Practice assignment.  This assignment is from the [Selectors](Selectors.md) Lesson.

1. Add 3 different psuedo-classes to your CSS file. Comment the code to explain what each of the psuedo-classes do.

> If you don't know how to do something right away, remember S.A.T.!!  Search for the answer in your textbook or Google, Ask your classmates and/or teacher, then Teach your solution. Another student may have the same question.

*****

### Know Your Docs

Be sure to reference the official documentation on [CSS Pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp) from W3Schools. Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

*****

## Questions for Class Discussion

1. What is the purpose of a psuedo-class?
1. How do you use a psuedo-class?
1. Name 5 different pseudo-classes and their purpose.

*****

### Terminology to Know

Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

* Pseudo-Class
* Selector
* Link
* Hover
* Visited

{% include "../includes/footer.md" %}
