# accessible name

An accessible name is the way in which assistive technologies primarily reference, or refer to, an element. Think of it like your own name, but instead of naming a living, breathing person, it’s used to name something like a button.

All of the interactive controls and components in our websites and applications need an accessible name, so that people can:
a. Understand what it is and what it might do
b. Understand how to refer to it

The accessible name might then be surfaced in a few different ways:
* People using screen readers will hear the accessible name when reading through the website, or when interactive with controls
* People using voice control software will use the accessible name to interact with the controls, for example: “Click, Buy now”

Therefore, a good accessible name is often **concise** and **easy to understand**.

## How does it work?

When our websites are rendered, the browser creates an accessibility tree, based on the page’s markup. The accessibility tree then contains a few different pieces of information about each element, including the accessible name!

## Adding an accessible name

In terms of how we provide the accessible name, there are a few different ways this works, and it can depend on the context of use.

### From a text node

Often, the text combined in the element will become the accessible name. In the following example, the accessible name will be “Save”.

```html
<button>Save</button>
```

### From CSS

Any text content provided using CSS’ pseudo elements can also factor in to the accessible name!

For example, if you’re appending or prepending content using the `::before` or `::after` pseudo elements, these may also make up part of your controls’ accessible names. 


