{% include "../includes/header.md" %}

# Animations - Part 2

## Transitions and Transformations

*****

**Objective:** By the end of this lesson, the student use transitions and transformations to add dynamic styles to a webpage.

**Assignment:** Boxes Animation Part 2

*****

## Transitions

  

The introduction of [Animate.css](https://animate.style/) is more of an introduction to a concept you'll be using throughout your coding journey, **open-source code**. Open-source means that is is open to public use and contribution. Within the JavaScript ecosystem, there have been over 350,000 code bases built for the use of anyone that wants to use them. So what does it mean to use other people's code? It means that you get do really cool things without having to do build the code yourself.  

I'm sure you're wondering how Animate.css comes into play with this **open-source** ecosystem. Turns out that animations, or movements on the page, are commonly used. Instead of re-building these animations from scratch, we can use the code built by Dan Eden!

*****

### Animate.css

The code for [Animate.css](https://github.com/daneden/animate.css) is held in online storage, just like all of your projects. Notice that the name has a `.css` file extension in it. This is because, it's **all CSS**!

You use it just like you use your own `.css` files, with a `<link rel="stylesheet" href="">` tag, but instead of `style.css` value in the `href=""` attribute you'll do this instead:

Because the source is online, we have to reference the url where it is found.
>***Remember**: the `<link>` tag is placed in `<head>` of the HTML file.*

| HTML for CDN Method to use Animate.css|
|----|

```html
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.2/animate.min.css">
</head>
<!-- This method requires an internet connection to work, even locally. -->
```

> ***NOTE** There is an updated version of Animate.css.  We are using an older version. Don't read the instructions on the Animate.css webpage. They are for the newer version that we aren't using, but the types of animations are the same.*  
*****

### Using Animate.css

Explore [Animate.css](https://animate.style/).  Use the right-hand navigation bar to test out the different animations.

The way to use **Animate.css** is to use the built-in class names. **Remember using classes?**  Each animation has a dedicated class name. Along with that, there is a specific syntax to writing the classes.  

>Add the class `animated` to an element, along with any of the animation names:

| Syntax for using Animate.css|
|----|
```html
<h1 class="animated bounce">An animated element</h1>
 
```

*This means this h1 element will 'bounce' when the page loads*

You need the `animated` class for each element you add an animation to.  You get to choose the animation name.

*****

### Timing and Repeats

Watch the video below for an introduction to how we customize our animations.  

<iframe width="560" height="315" style="margin-bottom:25px;" src="https://www.youtube.com/embed/2a2p2FhBgfA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

Notice in the video that there some properties that can be adjusted to customize your animation.

* **Delay Class**
    * Using the `delay` class will delay the animation until the specified time has passed.

        |  Class Name  |  Duration |
        |:-:|---|
        | `delay-2s`  |  2s |
        | `delay-3s`  |  3s |
        | `delay-4s`  |  4s |
        | `delay-5s`  |  5s |

* **Speed Class**
    * Using the `speed` class will delay the animation until the specified time has passed.

        |  Class Name  |  Duration |
        |:-:|---|
        | `slow`  |  2s |
        | `slower`  |  3s |
        | `fast`  |  800ms |
        | `faster`  |  500ms |

* **CSS Properties**
    * `animation-duration` : The amount ofntime it takes for the animation to complete.  This can slow the animation down.
    * `animation-delay` : The amount of time before the animation will execute on the webpage.
    * `animation-iteration-count` : The number of times that the animation will repeat.  

*****

### Practice It - [Boxes Practice](URLtoEXAMPLE1)

* The goal of this assignment will be to animate the boxes.
* Remember to **Fork!**
<iframe
     src="https://codesandbox.io/embed/animated-boxes-57xk2?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Animated Boxes"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

*****

### Know Your Docs - 

 
* [W3Schools Transitions](https://www.w3schools.com/css/css3_transitions.asp)
* [CSS Transitions/Transforms](https://thoughtbot.com/blog/transitions-and-transforms)

*****

### Push yourself further

* Animate the Practice Landing Page from the last lesson.
* Add animations to your Final Project webpage.
* Try updating your version to the newer version.  
    * There are more animations to use.
    * Be careful!  The syntax is different.

*****

### Terms to Know

* Open-Source
* `<link>`
* Class 
* `href` attribute
* Timing Functions
* Animation
* milliseconds

*****

## Questions for Student Discussion

1. What are some advantages of different code bases being **open-source?**
1. Explain how to add animations to HTML elements using [Animate.css](https://animate.style).
1. Can you add more than one animation to an element? *(Hint: Try it out)*
1. How are seconds and milliseconds related?


*****

### Let's go to the next Lesson [Animations Part 2 >](AnimationsPt2.md)

{% include "../includes/footer.md" %}
