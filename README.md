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

**Step 21**

There are two main color models: the *additive* RGB (red, green, blue) model used in electronic devices, and the *subtractive* CMYK (cyan, magenta, yellow, black) model used in print.

In this project, you'll work with the RGB model. This means that colors begin as black, and change as different levels of red, green, and blue are introduced. An easy way to see this is with the CSS `rgb` function.

Create a new CSS rule that targets the class `container` and set its `background-color` to black with `rgb(0, 0, 0)`.

**Step 22**

A function is a piece of code that can take an input and perform a specific action. The CSS `rgb` function accepts values, or arguments, for red, green, and blue, and produces a color:

Example Code

```rgb
rgb(red, green, blue);
```

Each red, green, and blue value is a number from `0` to `255`. `0` means that there's 0% of that color, and is black. `255` means that there's 100% of that color.

In the `.one` CSS rule, replace the color keyword `red` with the `rgb` function. For the `rgb` function, set the value for red to `255`, the value for green to `0`, and the value for blue to `0`.

**Step 23**

Notice that the `background-color` for your marker is still red. This is because you set the red value of the `rgb` function to the max of `255`, or 100% red, and set both the green and blue values to `0`.

Now use the `rgb` function to set the other colors.

In the `.two` CSS rule, use the `rgb` function to set the `background-color` to the max value for green, and `0` for the other values. And in the `.three` CSS rule, use the `rgb` function to set the `background-color` to the max value for blue, and `0` for the other values.

**Step 24**

While the red and blue markers look the same, the green one is much lighter than it was before. This is because the `green` color keyword is actually a darker shade, and is about halfway between black and the maximum value for green.

In the `.two` CSS rule, set the green value in the `rgb` function to `127` to lower its intensity.

**Step 25**

Now add a little more vertical space between your markers and the edge of the `container` element they're in.

In the `.container` CSS rule, use the shorthand `padding` property to add `10px` of top and bottom padding, and set the left and right padding to `0`. This works similarly to the shorthand `margin` property you used earlier.

**Step 26**

In the additive RGB color model, *primary colors* are colors that, when combined, create pure white. But for this to happen, each color needs to be at its highest intensity.

Before you combine colors, set your green marker back to pure green. For the `rgb` function in the `.two` CSS rule, set green back to the max value of `255`.

**Step 27**

Now that you have the primary RGB colors, it's time to combine them.

For the `rgb` function in the `.container` rule, set the red, green, and blue values to the max of `255`.

**Step 28**

*Secondary colors* are the colors you get when you combine primary colors. You might have noticed some secondary colors in the last step as you changed the red, green, and blue values.

To create the first secondary color, yellow, update the `rgb` function in the `.one` CSS rule to combine pure red and pure green.

**Step 29**

To create the next secondary color, cyan, update the `rgb` function in the `.two` CSS rule to combine pure green and pure blue.

**Step 30**

To create the final secondary color, magenta, update the `rgb` function in the `.three` CSS rule to combine pure blue and pure red.