# CSS-Accordions
A simple and elegant solution for accordion elements using only HTML and CSS. Create collapsible bulleted lists without JavaScript.
<br />
Based on the excellent ['CSS + HTML only Accordion Elements'](https://codepen.io/abergin/pen/ihlDf) by [Alex Bergin](https://codepen.io/abergin/).


### Features

* Create accordion elements within bulleted lists using only CSS and HTML. This is ideal for situations where JavaScript must be avoided (for example, on the basic hosting plan from Squarespace)
* Uses a simple text label to open/close the accordion, and updates the label to reflect the current status of the element (open or closed)
* Allows for identation of nested elements
* Only requires a minimal number of specialized CSS classes in order to function

### How it Works

* Uses the `:checked` attribute and the `~` sibling selector to apply different styles based on the status of a hidden checkbox (checked or unchecked)
* The hidden check box is placed over the text we want to use as a button using `position: absolute`. This effectively turns the text into a button.
* If the `:checked` attribute is not supported the code degrades gracefully into a standard, fully expanded list
* Bulleted lists are created by treating `p` paragraphs contained within a standard unordered list as `list-items` because hiding individual `li` elements is not possible without JavaScript (to my knowledge)

An example of this code in action can be found here: [Link to CodePen.io](https://codepen.io/togden/pen/xMRbrx)


