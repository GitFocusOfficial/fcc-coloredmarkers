# Learn CSS Colors by Building Colored Markers

Selecting the correct colors for your webpage can greatly improve the aesthetic appeal to your readers.

In this course, you'll build a set of colored markers. You'll learn different ways to set color values and how to pair colors with each other.

**Step 1**

As you've seen in the previous projects, webpages should start with a DOCTYPE html declaration, followed by an html element.

Add a DOCTYPE html declaration at the top of the document, and an html element after that. Give the html element a lang attribute with en as its value.

**Step 2**

Nest a head element within the html element. Just after the head element, add a body element.

**Step 3**

Remember that the title element gives search engines extra information about the page. It also displays the content of that title element in two more ways:

- in the title bar when the page is open
  
- in the browser tab for the page when you hover on it. Even if that tab is not active, once you hover on the tab, the title text is displayed.

Within the head element, nest a title element with the text Colored Markers.

**Step 4**

The charset attribute specifies the character encoding used by the document. utf-8 (Unicode Transformation Format – 8-bit) is a character encoding standard used for electronic communication.

Inside the head element, nest a meta element with the attribute charset set to "utf-8".

**Step 5**

You can have multiple meta elements on a web page. Each meta element adds information about the page that cannot be expressed by other HTML elements.

Add another meta element within the head. Give it a name attribute set to "viewport" and a content attribute set to "width=device-width, initial-scale=1.0" so your page looks the same on all devices.

**Step 6**

Now you're ready to start adding content to the page.

Within the body, nest an h1 element with the text CSS Color Markers.

**Step 7**

In this project you'll work with an external CSS file to style the page. We've already created a styles.css file for you. But before you can use it, you'll need to link it to the page.

Nest a link element within the head element. Give it a rel attribute set to "stylesheet" and an href attribute set to "styles.css".

**Step 8**
Now that your external CSS file is set up, you can start styling the page.

As a reminder, here's how to target a paragraph element and align it to the right:

Example Code

```p
p {
  text-align: right;
}
```

Create a new CSS rule that targets the h1 element, and set its text-align property to center.

**Step 9**

Now you'll add some elements that you'll eventually style into color markers.

First, within the body element, add a div element and set its class attribute to container. Make sure the div element is below the h1 element.

**Step 10**

Next, within the div element, add another div element and give it a class of marker.

**Step 11**

It's time to add some color to the marker. Remember that one way to add color to an element is to use a color keyword like black, cyan, or yellow.

As a reminder, here's how to target the class freecodecamp:

Example Code

```free
.freecodecamp {
  
}
```

Create a new CSS rule that targets the class marker, and set its background-color property to red.

Note: You will not see any changes after adding the CSS.

**Step 12**

The background color was applied, but since the marker div element has no content in it, it doesn't have any height by default.

In your .marker CSS rule, set the height property to 25px and the width property to 200px

**Step 13**

Your marker would look better if it was centered on the page. An easy way to do that is with the margin shorthand property.

In the last project, you set the margin area of elements separately with properties like margin-top and margin-left. The margin shorthand property makes it easy to set multiple margin areas at the same time.

To center your marker on the page, set its margin property to auto. This sets margin-top, margin-right, margin-bottom, and margin-left all to auto.

**Step 14**

Now that you've got one marker centered with color, it's time to add the other markers.

In the container div, add two more div elements and give them each a class of marker.

**Step 15**

While you have three separate marker div elements, they look like one big rectangle. You should add some space between them to make it easier to see each element.

When the shorthand margin property has two values, it sets margin-top and margin-bottom to the first value, and margin-left and margin-right to the second value.

In your .marker CSS rule, set the margin property to 10px auto.

**Step 16**

To give the markers different colors, you will need to add a unique class to each one. Multiple classes can be added to an element by listing them in the class attribute and separating them with a space. For example, the following adds both the animal and dog classes to a div element.

Example Code

```div
<div class="animal dog">
```

If you add multiple classes to an HTML element, the styles of the first classes you list may be overridden by later classes.

To begin, add the class one to the first marker div element.

**Step 17**

Next, remove the background-color property and its value from the .marker CSS rule.

**Step 18**

Then, create a new CSS rule that targets the class one and set its background-color property to red.

**Step 19**

Add the class two to the second marker div, and add the class three to the third marker div.

**Step 20**

Create a CSS rule that targets the class two and set its background-color property to green.

Also, create a separate CSS rule that targets the class three and set its background-color to blue.