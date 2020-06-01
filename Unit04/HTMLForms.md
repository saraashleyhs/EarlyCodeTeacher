{% include "../includes/header.md" %}

# HTML Form Elements

*****

**Objective:** By the end of this lesson, the student will create and style an HTML form.

**Assignment:** NASA Page Practice

*****

### What is an HTML Form Element?

Forms are probably the most common element we interact with on a web page.You will see them as a search bar, contact form, sign-up/log-in, or an application form.   Anywhere that a website captures data given to us from a user and does something with it, is done using forms.

While we're not going to get into storing or manipulating the data in this course, it's important we grasp how to capture the data in the browser, **validate** it, and really understand that these processes are so common that they've been built into the HTML structure and all we have to do is learn to search for their name and use them. Just like other properties you've learned to use throughout theis course, the special **attributes** and dedicated form elements are just more *things* you can use to build impressive and functional web pages.

Before we begin, just like the `<table>` element has dedicated child elements like `<tr>`, `<th>`, `<td>`, etc, the `<form>` element also has dedicated child elements like `<label>`, `<input>`, `<button>`, etc. And each of those elements has dedicated **attributes**. Attributes, for all intents and purposes, are just another word for **property**. They are a place we can store values on the *object-thing* we're working with. So when we want our `<input>` element to take in numbers instead of letters we change the `type=` attribute, see below:

| HTML |
|----|

```html
<!-- for number data -->
<input type="number">

<!-- or for text data -->
<input type="text">
```

The input field will look the same on the webpage but now the type of data allowed to go into them will be different, numbers for the first `input` and letters for the second `input`.

<!-- ### Context Video -->
<!-- @TODO @CLAYTON ADD screen share video on forms and inputs -->

#### The `<form>` Element

The `form` element doesn't have a physical representation on the screen. Instead it only defines a place for us to store data that can be retrieved easily and sent to a server. So again, it's just creating another *object-thing* on the Document *object-thing* where we can store data. To define places for that data to be stored within it we use its dedicated child elements.

**Form Elements** include: `<input>` & `<label>`, `<textarea>`, `<select>`, `<fieldset>` & `<legend>`, `<datalist>`, and `<output>`.

Each of these elements perform various actions which we'll cover in detail below. But an example of how you'd create a `form` element is shown below:

| HTML for `form` Element|
|----|

```html
<form action="results.html" method="GET">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

> *NOTE 1: The `<br>` tag stands for "Break". It forces a line-break on the page so that each of these **Inline Elements** don't jam-up on each other on one line.*
> *NOTE 2: the `action=` & `get=` attributes are covered in the "Suggested Viewing" video below. For now, just know they tell the browser where to send the stored data and how to send the stored data.*

##### The `<input>` & `<label>` Elements

These two elements always go together. While `<input>` elements create a place for the user to input data and see it on the screen, the `<label>` elements *label* the `input` element both for the user to see on the screen as well as the data we store with it under-the-hood. A common example is shown below:

| HTML for `input` Element|
|----|

```html
<form>
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="user"><br>
</form>
```

The HTML snippet above has a `<label>` element with the `for` **attribute** set to `"username"`. In this way it is now tied to the `input` element next to it with the `id="username"` and **NOT** the `name` or `type` attributes. You see that? The label is `for` the `id` of the input.

###### The `<input>` Attributes

As we've stated before, the Form Elements have lots of specialized attributes. We won't cover all of them because you can reference your docs as you grow as a developer later on but today, we'll introduce a few of the common ones so you can apply them in class tomorrow. The list below tells you all of the values you can give to the `type` attribute of an `input` element.

* `<input type="text">`: defines a one-line text input field. If you need a bigger area for lots of text you'll use a `<textarea>` element.
* `<input type="password">`: defines a password field.
* `<input type="submit">`: defines a button for submitting form data.
* `<input type="radio">`: defines a radio button.
* `<input type="checkbox">`: defines a checkbox.
* `<input type="button">`: defines a button.
* `<input type="date">`: creates a date selector
* `<input type="submit" value="Submit">`: creates a button that is registered automatically with its parent `form` element as a "Submit" button *AND it doesn't need a `label` partner.*

Remember to pair every `input` element **needs** a `label` element that has a `for` attribute to match its `id` attribute:

| HTML for `label`/`input` Pair|
|----|

```html
<form>
  <label for="phone-number">Phone:</label><br>
  <input type="number" id="phone-number" name="phoneNumber"><br>
  <input type="submit" value="Submit">
</form>
```

###### The `name` Attribute

Since we're saving data with our forms we have to know what the *name* of our data is. You get to determine this with the `name` attribute. While the `for`/`id` relationship is important, you have to also give your `input` elements a `name` attribute because this is how you will access the data later. Think of it like creating your own property *names* like: `innerHTML`, `color`, `font-family`, etc. Every `input` will have a unique name with one exception, the `type="radio"` input.

The `type="radio"` input will all share the same `name` attribute because they can only be saved to 1 value.

| HTML for `radio` Button |
|----|

```html
<form>
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Male</label><br>
  <input type="radio" id="female" name="gender" value="female">
  <label for="female">Female</label><br>
  <input type="radio" id="other" name="gender" value="other">
  <label for="other">Other</label>
</form>
```

Notice how all the radio buttons have the same `name` attribute, "gender"? This is because no matter what the user selects it will be saved to the `name` slot of the form.

###### Other `input` Attributes

**Data Validation** or **Form Validation** means we're verifying the data a user puts in such as the type, length, validity, and shape we want it so we can properly save it to a database.

It is costly both in time and money to send the data from the user to our databases only for it to be in the wrong format. A shorter, safer, and cheaper first "filter" we can use is HTML's built-in **Form Validation** and you've actually already seen one of the tools, `type`, which specifies the *type* of data that can go into an input.

Look at a few of the following attributes we can leverage on `input` elements.  Reference the *docs* section for more information on these attributes.

* `maxlength=`: limits the maximum number of characters that can go into the input
* `minlength=`: limits the minimum number of characters that can go into the input
* `max=` and `min=`: creates upper and lower limits on a date input
* `required`: forces the user to fill out the input
* `email`: verifies that the input has a `@` and `.com`
* `phone`: verifies that it is a legit phone number
* `autocomplete="on"`: let's the browser offer autocompletion of the form
* `password`: blots out the characters in this field automatically
* `placeholder`: isn't a validation attribute but it does give the user a hint about what goes in the field

<!-- > *The last one is `pattern="[A-Za-z]{3}"`: the pattern attributes take RegEx to validate the input. This example says the input must be exactly 3 letters between A-Z either caps or lowercase. This is a very powerful attribute and not something you have to worry with for now, but we'll get into [RegEx](https://www.youtube.com/watch?v=r6I-Ahc0HB4) in your 200 level class so you'll be able to build some very powerful forms.* -->

##### Other Form Elements

Besides `input` there are a few other form elements you should know about but don't concern yourself with too much. Remember, there are a lot of tools built into HTML that were developed over years of trial and error and there is no way for us to learn every detail to perfection right now.  That is why we refer to the documentation.

* `<textarea>`: As mentioned before, is for large sections of text like this page you're reading now!!! ;)
This can be used for an "Additional Comments" section.
* `<datalist>`: give you a "pre-fill" menu for your `input`s
* `<output>`: of course, shows you the output of some script you've built.
* `<select>`: offers a dropdown menu to your user.

*****

## Button Element

As you learned earlier, `input` elements can be changed to accept all sorts of data including *buttons* by changing the value of their `type=` attribute. Here well cover the actual `<button>` element because the real reason to use it over a `<input type="button">` element is for styling.

If you're wanting to put content or images inside of a button then you'll have to use the `<button></button>` element. Plain and simple, that is it!

However, if you want to use a `<button>` element on a form you have to set its `type=` attribute to `"submit"`: `type="submit"` and *poof*, you have a submission button.

The last things we'll say about HTML Form Elements is that they can all be [styled just like your other HTML Elements](https://www.youtube.com/watch?v=2ACrHs5o9LM). Have fun, let your creativity run wild, and enjoy building!!

******

## Practice It

Try working with this [Example Form CodeSandbox](https://codesandbox.io/s/forms-example-qf090?fontsize=14&hidenavigation=1&theme=dark).
* Explore some of the elements that have been explained in this lesson.

 <iframe
     src="https://codesandbox.io/embed/forms-example-qf090?fontsize=14&hidenavigation=1&theme=dark"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Forms Example"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

#### Assignment

### Wireframe the [NASA Web Page](../images/homework.jpg) - 15 mins

Using the [NASA Mockup](../images/homework.jpg), the instructor will lead a whiteboarding session teaching students how to wireframe so that students understand the importance and usefulness of planning before coding.

![NASA Mockup](../images/homework.jpg)

******

### Build the NASA Page

This project will bring together several topics that we have learned so far.  You will use Flexbox or Grid, adding images, the Box Model, etc. to complete this assignment.
**Fork** the [NASA CodeSandbox](https://codesandbox.io/embed/floral-sunset-e9hpi?fontsize=14&hidenavigation=1&theme=dark)

1. Draw a wireframe with HTML tags denoting each element
1. Using `display: flex;` and the Box Model, follow the mock-up below to build the NASA landing page.
1. Use [ColorPick Eyedropper](https://chrome.google.com/webstore/detail/colorpick-eyedropper/ohcpnigalekghcmgcdcenkpelffpdolg?hl=en) to get the right colors.
1. Use a `<form>` and `<input>` elements to create the form in the mockup.

*****  

## Know Your Docs

* [HTML Form Elements](https://www.w3schools.com/html/html_forms.asp)
* [Input Attributes](https://www.w3schools.com/html/html_form_attributes.asp)
* [Styling Form Elements](https://www.w3schools.com/css/css_form.asp)
* [Why use `<button>` over `<input type="button">`](https://www.geeksforgeeks.org/button-tag-vs-input-typebutton-attribute/)?

### Suggested Viewing

* [HTML Form Elements in 25 mins](https://www.youtube.com/watch?v=fNcJuPIZ2WE)
* [HTML5 Form Validation](https://www.youtube.com/watch?v=bb4NqVycr-4)

*****

## Terms to Know

* Attribute
* Form Validation
* Data Validation
* Client-side Validation
* `<button>` Element

*****

## Questions for Student Discussion

1. What makes the `form` element special? How does it store data?
1. Can you describe the way the `input` attribute: `name` creates a place for data to be stored on the `form` element-*object-thing*?
1. What is a property? How is it similar to an attribute?
1. Why do we need to validate our data?
1. What does the `<br>` element do?
1. What is an inline element?

*****

### Let's go to the next Lesson [Linking Pages >](ExternalResources.md)

{% include "../includes/footer.md" %}