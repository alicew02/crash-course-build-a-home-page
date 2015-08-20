## Campus Overview

**Duration:** 3hrs

**Copy for Meet-up page:**



## Instructor Overview
This overview informs instructors on how to teach this crash course in approximately 3 hours. The structure of this crash course is part lecture and part assignment. The objective is for students to leave the crash course with a completed web page, built with basic HTML, CSS, and JavaScript.

## Key Concepts (Agenda)


1. [Setup](#setup)
2. HTML Tags and whitespace
 1. Attributes
3. [Basic CSS](#css)
 1. Tag Selectors
 1. Class Selectors
 1. Nesting HTML
1. [Project](#project)
 1. Introduce the HTML
 1. Design the Header
1. [Extra Learning with JavaScript](#jsExtra)

<a id="setup"/>
## Setup

To start, it's recommended that students download [SublimeText](http://www.sublimetext.com/2) prior to attending. It's also recommended that the students use [Chrome]() or [Firefox]() when doing the Workshop.

Set up folder structure with the following files and explain their purpose

    - index.html
    - css
        - styles.css
    - scripts
        - main.js

## HTML Tags and Whitespace

Start your HTML file by typing only plain-text. Show that this can be saved and rendered in the browser. Show that things like hard returns and duplicate spaces don't really matter (whitespace is ignored).

After showing plain-text, show how simple tags like `<p>` and `<h1>` can be used to enhance our document. Explain the "anatomy" of a tag and how opening/closing tags work. Using paragraph tags are nice because you can demonstrate how space is created between the content when rendered.

### Attributes

Explain that attributes enhance tags and give them more abilities. Anchor tags are a great example of explaining attributes.

```html
<a href="http://theironyard.com">The Iron Yard</a>
```


At this point, your demonstration might look something like:

```html
<html>
<head>
    <title>Build A Web Page</title>
</head>
<body>
    <h1>Build a Web Page</h1>
    <h2>A crash-course with The Iron Yard</h2>

    <p>The objective is for students to leave the crash course with a completed web page, built with basic HTML, CSS, and JavaScript.</p>

    <a href="http://theironyard.com">The Iron Yard</a>
</body>
</html>

```

<a id="css"/>
## CSS

Show students how to create a CSS file in a `styles` folder and use a `<link rel="stylesheet" type="text/css" href="css/styles.css">` to link it.

### Tag Selectors

Introduce the basic concepts of inline vs block tags. It's important to stylize several paragraphs all to be `background-color: something` so the students can see that no matter how many tags we have, the CSS will apply to all that match.

### Class Selectors

Since we're at a point where we have all of our paragraphs stylized with one CSS block, it would be a good time to introduce the concept of classes and how to stylize a whole group of tags (as with all the paragraphs) and then to isolate certain ones with class names.

> Tip: Since the students are already familiar with tag selectors, it would be important to the syntax: `tag.class-name` instead of just `.class-name` so the students feel like they are adding to their already existing knowledge of tag selectors

## Nesting in HTML

So far we should only have simple tags in our HTML without nesting. Nesting might be difficult to explain without seeing colors applied to tags so it makes more sense to explain nesting after we've applied some CSS. One idea could be to wrap our paragraph tags in a div tag and then stylized our div with a background color.

It will be important to introduce terms like `parent`, `child`, `sibling`, and `container` at this point so the students can more easily converse with the instructors when the see the project.

<a id="project"></a>
# Project

This repo's [GH Pages](https://theironyard.github.io/crash-course-build-a-home-page/) contains all files students should need.

## Introduce the HTML

It will be important to show the students the project's HTML at this point. Since the project makes use of proper `<html>`, `<head>`, and `<body>` tags. It might be useful to explain those in an isolated file at first.

Show the students that there are very semantic tag names with easy-to-understand classes and how it's relatively easy to tell which parts of the HTML correspond to which parts of the design.

## Design the Header

To get the ball rolling, you'll want to design some of the project for them. You might want to do the header section and challenge the students to look at the final output (`final.html`), look at what we have so far with `index.html`, look at the HTML and CSS selectors and try to figure out what properties need to be applied. Once you get some working you can let the students finish it off while you help out any students with questions.

Teach the basic concept of a reset and how the asterisk selector is used to apply all styles. This is where you'll show that some styles like the font-family are applied to all areas with just one selector, and then can be override:

```css
* {
    vertical-align: top;
}
```

<a id="jsExtra"></a>
# Extra Learning with JavaScript and toggling

If you have time, you can teach the students some basic JavaScript concepts. Start by teaching the concept of state-management with class names. You might have styles applied to a paragraph which serve as a default state, but then having a `class="selected"` is a new visual state and we accomplish this with class names. You might need to introduce the concept of multiple class names in HTML and how to select something with multiple class names in the browser.

Notice that the sample includes a JS file. In that JS you'll notice a simple event handler for when boxes get clicked. You can show the basics of how jQuery works with events and how classes can be toggled on and off of DOM elements with the "add spinkles button in the footer".
