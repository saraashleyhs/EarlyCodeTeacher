{% include "../includes/header.md" %}

# Pics, Links, and Videos

*****

**Objective:** By the end of this lesson, the student will add images, hyperlinks, and videos to a webpage.

**Assignment:** Digital Billboard

*****

### Overview

HTML is the only language that web content is encoded in. No matter what programming language you work in, if you're building stuff through the web you'll be encoding that software's content in HTML. Because HTML is the only language for the web, it has to be super flexible to handle all the of the crazy cool stuff we see on the web. *Just stop and think for a moment about some of the coolest websites you've seen.* All of that was built in HTML!!

So when you're wondering when you'll know everything there is to know about HTML, well maybe never.... But the upside to that is that there is always something to learn! So this week we'll spend time on some of the more special elements of HTML: `<img>`,`<iframe>`, and `<a>`. These will help you build more compelling websites!

Remember the tags that we use in our HTML have meaning.  The browser reads the tags that we use and interprets the type of content in them.  This is why it's important to use tags that correspond to the content that will go inside the element. A `<div>` will allow us to group or encapsule common elements on a page. A `<p>` is meant to hold text in groups of 'paragraphs'.

*****

## Part 1: Images

You probably recognize this element from a previous assignment, or even your own final project page. Today we'll look at the `<img />` tag more closely.

The `<img />` is a [self-closing](http://xahlee.info/js/html5_non-closing_tag.html) element that requires two attributes: `src=""` and `alt="A description to replace the image"` to look like the following code snippet:

```html
<img src="./images/grapefruit-slices-332.jpg" alt="Grapefruit slice atop a pile of other grapefruit slices."/>
```

* The `src=""` attribute(*source*) takes a **URL** or **pathname** to tell the browser where to find the image file.

<br>

* The `alt=""` attribute(*alternative text*) is used in place of the image when it is not being displayed or when someone with a visual impairment visits your page. This "alt" text is **required** for **screen readers** — accessibility devices used primarily by the visually impaired — to be able to communicate image content to their users. For this reason you should include lengthy and descriptive alternative text so that screen readers can actually communicate what is in the image.

> *NOTE: I think it's important to know that a **pathname** and a **URL** are almost the same thing except...
> * A **pathname** refers to a path to a file that you have downloaded on your computer or stored in the project folder.
> * A **URL** refers to a path from a file on your computer to a file on another computer that is connected to your computer through the internet.

Check out this [video](https://youtu.be/X7uSEH5Dz5o) to learn how to add images to your project.

<iframe width="560" height="315" src="https://www.youtube.com/embed/X7uSEH5Dz5o" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

#### Best Practices

When you add images to your websites, it best to create an 'images' folder **within** the websites folder. Place all of your image files within that new folder. This makes sure that all of your project files stay all together.

You want to choose images that are available to be used or get permission from the resource owner to use that resource.  There are places that you can download free stock images.

Check out our [Resources](../preCourseWork/Resources.md) section.

> Hint: When you adjust the size of a pic, either adjust the height or the width property.  If you give values to both, it can distort the picture's appearance.

*****

## Part 2: Anchor Elements

An anchor element allows us to create a hyperlink to another location.  We use these elements to navigate to different websites or webpages.  

The `<img />` needed a `src` attribute to provide the image we want to display. Similarly, the anchor tag `<a>` needs an `href` attribute - a _**h**ypertext **ref**erence_ - if we want it to link to another location. You have seen the `href` attribute when we linked our CSS file to our HTML document.

```html
<a href="https://google.com">Search the web!</a>
```

Usually we see these elements as part of a navigation bar on a webpage.

> ProTip: To keep users on your webpage as long as possible, you don't want to force users to navigate away from your page.  To avoid this, use the `target` attribute.  
> `<a href="https://google.com" target="blank">Search the web!</a>` <pre>   target="blank" means that the link will be opened in a new tab.</pre>

*****

## Part 3: Videos - `<video>` & `<iframe>` Tags

Continuing on with adding media to our webpages, we're going to cover two important elements: `<video>` & `<iframe>`. These elements are similar to the `<img/>` element but have some funny but useful attributes to *play* with.
  
*****

### The `<video>` Element and its Attributes

The `<video>` tag creates an HTML element that will embed a media player into a page. This allows the user to interact with video playback inside the `document`. In order to use the video tag, you need to own the content and have the file downloaded in your project.

Just as you learned with the `<img />` element, the video element will get its content from a `src=""` attribute. Videos also come with the `width` & `height` attribute just like the `<img/>` element. But a few attributes you haven't seen before include:

* `autoplay` - sets the element's `autoplay` property to `true` which tells the browser to play the video as soon as the page loads.
* `controls` - sets the element's `controls` property to `true` which provides built-in play/pause buttons and a tracking slider.
* `poster` - means *thumbnail*, which is the initial image you see before a video plays. If this attribute isn't specified (left out of the tag) the browser will use the first frame in the video. This attribute takes a pathname or URL. 
* `muted` - sets the element's `muted` property to `true` which means the video will begin with no volume.
* `loop` - sets the element's `loop` property to `true` which means the video will play again when it finishes.

|HTML for Video Element|
|----|

```html
<video src="./videos/myMovie.mp4" width="320" height="240" poster="./images/myMovieThumbnail.png" autoplay controls><video>
```

*****

### The `<iframe>` Tag

So the `<video>` element is pretty straight-forward but remember, it is only used when you *own* the content, as in, it resides on your server. So what do you do if you don't own the content? Say for a youTube video? We'll, that's where we use an [Inline Frame element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe).

The `<iframe>` represents a nested browsing window, which effectively embeds another HTML page within the current page. You can include any number of `<iframe>` elements inside the `<body>` of a document, each of them displaying a separate page in the area covered by the `<iframe>`. While it can be used to display video, the `<iframe>` can **also** be used for things like games, code snippets for CodeSandbox, and advertising. When it comes to video, `<iframe>` is used primarily when we are linking to the video on YouTube rather than storing the file in our project.

#### You Should Know

There are some security risks involved with the `<iframe>` element. The risk revolve around the fact that you are "effectively embed[ding] another HTML page within the current page". We won't go into the technicalities of this because it is beyond the scope of this course but you should be aware as you move forward. Read this short article, [3 Reasons You Might Not Want To Use Iframes](https://www.ostraining.com/blog/webdesign/against-using-iframes/) by Alex Smirnov to get an idea of the problems surrounding the special element.

**Embedding videos from Youtube:**
> Youtube actually creates the `<iframe>` for us.  When you find a video you like:
> * Click on *Share* <pre> <img height="50" src="../images/YoutubeShare.png"></pre>
> * Click on *Embed* <pre> <img height="95" src="../images/YoutubeEmbed.png"></pre>
> Then you can copy and paste the `<iframe>` element directly into your HTML code.

*****

### Suggested Viewing

* [Video Element](https://youtu.be/Ynuz1UGPoTg)
* [Responsive Iframe](https://youtu.be/9YffrCViTVk)
* **HIGHLY SUGGESTED**: [Video vs Iframe Element](https://www.youtube.com/watch?v=OOy764mDtiA)

> *NOTE: In the last video you'll learn about the CSS property `position` which is very useful hack to making element do what we want!*

*****

## Practice It - Digital Billboard [CodeSandbox](https://codesandbox.io/s/digital-billboard-g8b6d?fontsize=14&hidenavigation=1&theme=dark)

1. Choose a local business that you would like to create a Billboard for.  

1. Search for content using our [Resources](../preCourseWork/Resources.md).

1. Fork the CodeSandbox and Add the content to the Billboard Template

<iframe
     src="https://codesandbox.io/embed/digital-billboard-g8b6d?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Digital Billboard"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

> If you don't know how to do something right away, remember S.A.T.!!  Search for the answer in your textbook or Google, Ask your classmates and/or teacher, then Teach your solution. Another student may have the same question.

*****

### Know Your Docs

Resources on [W3Schools]() and [Youtube](www.youtube.com):

* [Hyperlinks](https://www.w3schools.com/html/html_links.asp)
* [Images](https://www.w3schools.com/html/html_images.asp)
* [HTML Image Tag](https://www.w3schools.com/tags/tag_img.asp)
* [HTML 'a' tag](https://www.w3schools.com/tags/tag_a.asp)
* [iFrames](https://www.w3schools.com/tags/tag_iframe.asp)
* [Adding Images](https://youtu.be/_w6N_nplmAw)

*****

## Questions for Class Discussion

1. Describe the different tags used for adding media to a webpage.
1. How do you add a hyperlink?
1. What are the 2 ways to add images to your project?
1. Can you change the size of pics and videos on your webpage?

*****

### Terminology to Know

Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

* img tag
* Declaration
* Selector
* Link
* Property
* Value

*****

### Let's go to the next Lesson [Pseudo Classes >](PseudoClass.md)

{% include "../includes/footer.md" %}
