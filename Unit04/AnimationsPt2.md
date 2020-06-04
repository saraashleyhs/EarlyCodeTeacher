{% include "../includes/header.md" %}

# Animations - Part 2

## Transitions and Transformations

*****

**Objective:** By the end of this lesson, the student use transitions and transformations to add dynamic styles to a webpage.

**Assignment:** Boxes Animation Part 2

*****

## Transitions

When we want to simulate movement on our webpage, we can use transitions and transformations to do this.  This is very similar to animations but we can customize and use multiple transition properties.A transition allows us to make those movements smooth and pleasing to the user's eyes.  Jerky and sharp movements can distract the user and take away from the User Experience(UX) design of the page.  For an introduction into what a transition looks like, watch the video below.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Nloq6uzF8RQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

*****

### Creating a Transition

In the video you were able to see some of those properties in action, now let's see how to code it ourselves.

In order to create a transition, you have to think about your starting state and ending state.  You also have to think about the specific CSS property that will be transitioning.  For example, if we wanted to change the size of the object, we would consider transitioning the width and the height.  

The following code represents a transition on a `div` element.

|  CSS  |
|----|

```css
div {
  width: 100px;
  height: 100px;
  background: blue;
  transition: width 2s;
}
```

This tells the browser that we will have a 2 second transition on the width.  But, it's missing something. The code block above only tells where the width value will begin.  We also have to specify the ending value.  So we need some more code.

```css
div:hover {
  width: 300px;
}
```

The transition will happen when the `div` element is hovered over.  The width started at `100px` and after 2 seconds will have a width of `300px`.

> *Note: You can change more than one property at a time by listing the properties using the transition CSS property.
```css
div {
  transition: width 2s, height 4s;
}
```

Almost all CSS properties can have a transition, however, there are some properties that cannot use the transition property, such as font. 

*****

### Transition Properties - [CSS Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

Just like with Animate.css, there are some properties that can be adjusted to customize your transition.

* [**Transtion Property**](https://www.w3schools.com/cssref/css3_pr_transition-property.asp)
    * `transition-property` is used to specify the name of the CSS property that the transition will apply to.

```css
    div {
      transition-property: width, height;
    }

    div:hover {
      width: 300px;
      height: 300px;
    }
```

Notice how there are 2 properties that will be transitioning.

#### Once you have specificed the properties that will be changing, you could adjust the timing of the transition.

* [**Transition Delay**](https://www.w3schools.com/cssref/css3_pr_transition-delay.asp)
    * All animations/transitions automatically begin as soon as the page loads, unless you specify a delay.
    * Can be written in milliseconds or seconds.

```css
    div {
      transition-delay: 200ms;
    }
```

Remember there are `1000ms` in `1s`.

* [**Transition Duration**](https://www.w3schools.com/cssref/css3_pr_transition-duration.asp)
    * This property specifcies how long the transition will last.
    * Can be written in milliseconds or seconds.

```css
    div {
      transition-duration: 350ms;
    }
```

* [**Transition Timing Function**](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)
    * This property allows you to customize the speed throughout the transition.
    * There are different types of timing functions and at a higher level, you would learn how to define your own.

```css
    div {
      transition-timing-function: ease-in;
    }
```

>**Built-in timing functions:** 
    >* `linear`
    >* `ease`
    >* `ease-in`
    >* `ease-in-out`
    >* `ease-out`

<br>

![Examples](../images/Timing_Functions_Demo.gif)

*****

## Transformations

*****

### Practice It - [Boxes Practice](URLtoEXAMPLE1)

* The goal of this assignment will be to animate the boxes.
* Remember to **Fork!** 
<iframe
     src="https://codesandbox.io/embed/animated-boxes-part-2-h2c8c?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Animated Boxes Part 2"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

*****

### Know Your Docs - 

* [CSS Transitions/Transforms](https://thoughtbot.com/blog/transitions-and-transforms)
* [W3Schools Transitions](https://www.w3schools.com/css/css3_transitions.asp)
* [Transition Timing Function](https://www.w3schools.com/cssref/css3_pr_transition-timing-function.asp)
* [W3Schools Transform](https://www.w3schools.com/cssref/css3_pr_transform.asp)
* [2D Transforms](https://www.w3schools.com/css/css3_2dtransforms.asp)
* [3D Transforms](https://www.w3schools.com/css/css3_3dtransforms.asp)


*****

### Push yourself further

* Add transitions and transformations to your Final Project webpage.
* Add 3D transformations to your webpage.
* Research how to create your own animations using `@keyframes`

*****

### Terms to Know

* Transition
* `transition-delay`
* `transition-duration`
* `transition-property`
* `transition-timing-function`
* `transform`
* `translate`
* `scale`
* `rotate`

*****

## Questions for Student Discussion

1. What are some advantages of different code bases being **open-source?**
1. Explain how to add animations to HTML elements using [Animate.css](https://animate.style).
1. Can you add more than one animation to an element? *(Hint: Try it out)*
1. How are seconds and milliseconds related?


*****

### Let's go to the next Lesson [Animations Part 2 >](AnimationsPt2.md)

{% include "../includes/footer.md" %}
