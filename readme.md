# Horiseon Homepage - Refactoring
## Description
For this project, I was tasked with refactoring the site's html and CSS to improve accessibility without changing its appearance. Some aspects (e.g. removing redundant classes/attributes) were relatively straightforward. Others, such as such as deciding on suitable 'alt' text for the page's images, proved to be more of an art than a science. 

---
## Accessibility improvements
$~$

**html elements** were originally non-semantic (e.g. '\<div>'). While some non-semantic elements remain, the following semantic elements have been added:
- \<header> - the top section of the page, housing the navigation links;
- \<nav> - within the header, housing the only interactive page elements;
- \<main> - the main page content featured below the hero image;
- \<section> - initially '\<aside>', however further research suggested this was not semantically appropriate for meaningful page content; and
- \<footer> - the bottom section of the page.  
$~$

**alt text** for images was originally descriptive (from top to bottom):
### \<main>
* "Exercise book surrounded by office supplies."
* "Worker holding phone and typing on laptop simultaneously."
* "Busy conference table with colourful social media icons."
### \<section>
* "Funnel with gear at top and money coming out bottom."
* "Suit jacket with light bulb in place of head."
* "Gear surrounded by coins."  

However, research into accessibility best practice suggested that decorative images should not be given descriptive alt text, as such descriptions do not enhance meaning. Therefore, the author has decided to include blank alt attributes (i.e. '\<img alt = "">) to best satisfy accessibility requirements.

$~$

A **hidden description** was added before the navigation links to explain that the links only redirect elsewhere within the page (rather than to an external document). The description is visible to screen readers, but does not display visually.

## Credits
All rights to the site are the owner's, and credit for the layout and design goes its original creator. The following resources were consulted when making decisions about best practice for various topics:


## Tests
