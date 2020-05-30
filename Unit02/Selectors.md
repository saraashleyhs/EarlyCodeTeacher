{% include "../includes/header.md" %}

# CSS Selectors

*****

**Objective:** By the end of this lesson, the student will apply styles by targeting HTML elements based their relationships with one another.

**Assignment:**
CSS Diner
Selectors Practice

*****

#### Review and Recap

Previously, we have covered how to write CSS rules to add some style to our webpage.
Remind yourself of the 3 parts of a CSS rule:

 <img style="margin:auto; width:200px" src="../images/css-rule-anatomy.jpg">

 We will focus on the selector piece of the rule.  


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


*****

## Practice It - [CSS Diner](https://flukeout.github.io/#)

1. CSS Diner 
    <iframe
     src="https://flukeout.github.io/#"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="CSS Diner"
     >
     </iframe>

   <br>

1. Go through each level to select the correct piece in the diner.  

1. Follow the instructions in the CodeSandbox to style the HTML elements.

> If you don't know how to do something right away, remember S.A.T.!!  Search for the answer in your textbook or Google, Ask your classmates and/or teacher, then Teach your solution. Another student may have the same question.

*****

### Know Your Docs

Be sure to reference the official documentation on [CSS on W3Schools](https://www.w3schools.com/css/default.asp) Tutorials. Documentation makes software useful. All *good* software comes with documentation so new developers can pick it up, learn quickly, apply, and even change it if needed.

******

## Questions for Class Discussion

1. What is a selector?
1. Name 5 different element relationships and how you would select them in your CSS.  
1. How would you use a class selector?  Where does the class go?
1. How would you use an id selector?  

*****

### Terminology to Know

Take a look at these terms. If you don't know or can't describe any of them, take some time to teach yourself. You're a developer, which means you're also learning to develop yourself.

* 
* Parent Element
* Selector
* Link
* Property
* Value

*****
<!--TODO Include the Cascade-->

### Let's go to the next Lesson [Pics, Vids, and Links >](MediaTags.md)

{% include "../includes/footer.md" %}
