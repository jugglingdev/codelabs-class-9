# Bookmarking App

This project was completed as a part of Chris Sev's [Getting Started with JavaScript](https://chrissev.gumroad.com/l/getting-started-with-javascript/) course in conjunction with the [Codefi CodeLabs](https://www.codelabsdash.com/) bootcamp curriculum.

## Table of Contents

- Bookmarking App
  - Table of Contents
  - The Project
    - HTML
    - CSS
    - JavaScript
  - Reflection
  - Acknowledgements

## The Project

The Bookmarking App features a pop up input box that lets the user enter a full website address and add it to a collection of clickable links.  Once added, clicking the link will take the user to the website.  If no longer needed, the links can be deleted individually.  Each bookmark is stored locally, so refreshing the page will not clear the list.

![Bookmarking App Demo](img/bookmarking-app-demo.gif)

### HTML

The HTML for this project is fairly simple.  There's a *floater* where the user types the bookmark link and the *bookmark list* with submitted links.  In order to create the effect where the bookmark list and background go dark when the floater input is selected, an *overlay* div is included as well.

### CSS

Continuing with the overlay, its `z-index` is set under the floater and above the bookmark list and background.  That way, when the floater is selected, the overlay's `opacity` changes to darken everything behind it.  The floater scales up in size and stands out on the page because it is the only part of the app that doesn't darken behind the overlay.

Another helpful feature was setting up a *default avatar* for each bookmark image.  If a website doesn't have an image, then the default avatar will appear.

For this CSS, I used a new selector, `input[type=text]`.  This syntax allows the developer to select a specific input type rather than just `inupt` alone.

At the end of the project, I added additional hover effects to improve the UX when removing bookmarks.  First, I made the padding around the 'X' a little bigger to offer more wriggle room when clicking on the 'X'.  Second, though the 'X' appears and turn gray when hovering hover a given bookmark, I made it even darker when hovering directly over the 'X' itself.  Both of these effects should help the user more easily remove bookmarks.

### JavaScript




class on body as conditional in CSS

pointer-events

local storage

map()

default parameter

setting option const bookmarks = JSON.parse(localStorage.getItem('books')) || []; 
in case nothing is there yet

e.target.matches('.glyphicon-remove')
neat way to check if mouse click was on a given element when the event listener is attached to a parent element

can pass in i as second parameter in map() as a handy way to add data-id custom attribute to later ID specific bookmarks

console.dir(element) to see everything you have access to

OpenGraph

## Reflection


## Acknowledgements

Shoutout to [Dominika Roseclay](https://www.pexels.com/photo/shallow-focus-photograph-of-daisy-flower-1166869/) for taking the flower photo used as a background in this project.

Shoutout to [Chris Sev](https://chrissev.gumroad.com/) for his course [Getting Started with JavaScript](https://chrissev.gumroad.com/l/getting-started-with-javascript/).  He does a good job simplifying JavaScript concepts and then applying them to projects like these.

Another shoutout to [Codefi CodeLabs](https://www.codelabsdash.com/) for putting together this course and pulling in the best resources for learning software development.  The code coaches and this semester's cohort have been awesome to work with.
