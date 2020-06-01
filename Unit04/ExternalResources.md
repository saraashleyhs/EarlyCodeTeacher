{% include "../includes/header.md" %}

# Linking Pages 

*****

**Objective:** By the end of this lesson, the student will create and link multiple HTML pages together.

**Assignment:** Landing page practice

*****

### WebPage vs. Website

You have probably heard these terms used interchangeably but they actually do mean different things.  

A *webpage* is a single component as part of a *website*.  For example, if you look up something online and it takes you to a `Wikipedia.org` link, then you are viewing only one page on the entire Wikipedia site.  A *website* is really  talking about multiple webpages linked together.  So, the website `Wikipedia.org` has millions of single webpages that are linked together.  

You can have multiple HTML files in a project that can house a different component of your website.  You could also have multiple CSS files in your project. Today we will take a look at how we can do this with our projects.

*****

### Creating SubPages

When we first started creating CSS files that would be used to style our HTML pages, we had to link them together using a `<link>` element in our HTML.  This one CSS file doesn't have to be the only thing that is linked to our HTML.  

Generally, when you visit a website, we are navigated to what is called a **home-page** or a *landing-page*.  This is also called a *root directory*. Our homepage will always be The homepage is the base component for the website and usually contains navigation elements to the other webpages and overview content.

The homepage can naviagate to secondary pages in a project.  This is a subpage of the homepage. 
Watch this video on how to create subpages:

<iframe width="560" height="315" src="https://www.youtube.com/embed/lkDrG7G77Fg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

*****

#### The `<nav>` Element

Most websites have some sort of navigation bar on their homepages. These usually give links to other pages/resources that are a part of the site.  We need to make sure that the webpages are linked together so that we can use the navigation bar effectively.

Take a look at an example of a `nav` element below:

| HTML|
|----|

```html
      <nav>
        <a href="#">HOME</a>
        <a href="./aboutMe/aboutMe.html">ABOUT ME</a>
        <a href="./blog/EarlyCodeBlog.html">BLOG</a>
        <a href="./contact/index.html">CONTACT</a>
      </nav>
```

Notice we are using anchor tags nested within the `<a></a>` element to link to other resources here. The `nav` element does not link the other resources by itself. The `a` element works the same way as it would with a hyperlink to an external website, except this time the resource we are linking to is already inside of our project.

The `href` attribute is used here is find the **path** to the file that we are wanting to link to. The `#` on the `HOME` link means that this is the **root** directory. The `./` on the rest means that the file we are trying to find is on the same level as the file we are currently in. After that, is the rest of the **file-path** to the resource you need.  

*****

#### Practice It

We will use this project for our assignment.  Watch the video first to follow along with the steps.

<iframe width="560" height="315" src="https://www.youtube.com/embed/iXSSHlOe47s" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The video directions might be slightly off from what you will have to do only becuase we are using a different CodeSandbox.

*****

### Landing Page Practice

The goal is to create a navigation bar with nested anchor tags.

1. **Fork** the Landing Page [CodeSandbox](https://codesandbox.io/s/cold-rgb-njjxi?fontsize=14&hidenavigation=1&theme=dark)
1. The files are all created.  Your job is to link them together.
1. Follow the instructions in the CodeSandbox.

## Know Your Docs

* [HTML File Paths](https://www.w3schools.com/html/html_filepaths.asp)
* [Links](https://www.w3schools.com/html/html_links.asp)
* [HTML Lists](https://www.w3schools.com/html/html_lists.asp)

*****

## Terms to Know

* Web*Page*
* Web*Site*
* `a` Element
* `href` attribute
* File Path

*****

## Questions for Student Discussion

1. How do you know when to use `./` or `../` when getting a file path?
1. What does an anchor tag do?
1. How many pages could you link together

*****

### Let's go to the next Lesson [Animations >](AnimationsPt1.md)

{% include "../includes/footer.md" %}