# Horiseon Homepage - Refactoring
## 📚 Table of Contents
  - [💬 Description](#-description)
  - [♿ Accessibility improvements](#-accessibility-improvements)
  - [🏆 Credits](#-credits)
    - [Introductory Content](#introductory-content)
    - [HTML Semantic Elements](#html-semantic-elements)
    - [Hiding Content Accessibly](#hiding-content-accessibly)
    - [Alternative Text](#alternative-text)
    - [Resources](#resources)

## 💬 Description
For this project, I was tasked with <span style="color:orange">refactoring</span> the site's html and CSS to improve accessibility without changing its appearance. Some aspects (e.g. removing redundant classes/attributes) were relatively straightforward. Others, such as such as deciding on suitable 'alt' text for the page's images, proved to be more of an art than a science. 

---
## ♿ Accessibility Improvements

<span style="color:orange">Title</span> and <span style="color:orange">meta</span> tags were added to the head, including a page description and viewport instructions (for smaller devices).

<span style="color:orange">HTML elements</span> were originally non-semantic (e.g. '\<div>'). Some non-semantic elements remain, however the majority have been altered to reflect the nature of their content.

<span style="color:orange">Alternative text </span>for images was originally descriptive (from top to bottom):
    
    "Exercise book surrounded by office supplies."
    "Worker holding phone and typing on laptop simultaneously."
    "Busy conference table with colourful social media icons."

    "Funnel with gear at top and money coming out bottom."
    "Suit jacket with light bulb in place of head."
    "Gear surrounded by coins."  

However, none of the images on the page add meaning to the content they accompany). Therefore, the author has decided to use blank alt attributes (i.e. '\<img alt = "">) after consulting accessibility best practice resources.

An <span style="color:orange">aria-label</span> was assigned to the emoji heart in the footer to convey its meaning to screen readers.

A <span style="color:orange">hidden description </span> was added before the navigation links to explain that they only redirected focus elsewhere on the same page (rather than externally). The description is visible to screen readers, but does not display visually.

---
## ☑️ Tests
The site's accessibility was periodically tested using the WAVE Web Accessibility Evaluation Tool and Chrome's Lighthouse Web Developer Tool. Links to access these resources have been listed below.

### WAVE:
<img src="assets\images\wave.png" />

### Lighthouse:
<img src="assets\images\lighthouse.png" />

---
## ⌚ Future Improvements
Accessibility could be improved for visually-impaired persons by increasing the <span style="color:orange">contrast</span> between the font and background colour for the sidebar and footer sections. 

The site's sluggish performance limits accessibility for users with slower internet connections or less powerful devices. Lighthouse suggests the <span style="color:orange">bulky images</span> are the main culprits, and could be improved in the following ways:

<img src="assets\images\image_shrink.png" />

---
## 🏆 Credits
All rights to the site are the owner's, and credit for the layout and design goes its original creator. The following resources were consulted when making decisions about best practice for various topics:

### Introductory Content
- [Introduction to Web Accesssibilty - WebAIM](https://webaim.org/intro/)
- [HTML Accessibility - w3schools](https://www.w3schools.com/html/html_accessibility.asp)
- [8 things we can do to improve web accessibility - Prototypr.io](https://blog.prototypr.io/8-things-we-can-do-to-improve-web-accessibility-4774cc885b8d)
- [A primer on the noble craft of refactoring](https://www.tygertec.com/refactoring-primer/)
- [Understanding Assistive Technology: How Does a Blind Person use the Internet?](https://www.levelaccess.com/understanding-assistive-technology-how-does-a-blind-person-use-the-internet/)

### HTML Semantic Elements
- [HTML Semantic Elements - WebAIM](https://www.w3schools.com/html/html5_semantic_elements.asp)
- [Semantic HTML for Meaningful Webpages: Why Using Semantic Markup is Important in Web Design and Development - Brevity](https://www.w3schools.com/html/html5_semantic_elements.asp)
- [HTML5 semantic elements and Webflow: the essential guide](https://webflow.com/blog/html5-semantic-elements-and-webflow-the-essential-guide)
- [HTML5 Aside Element: Here Are The Good (And Not So Good) Uses For It](https://www.nomensa.com/blog/how-improve-web-accessibility-hiding-elements)

### Hiding Content Accessibly
- [A New and Easy Way to Hide Content Accessibly - Medium](https://medium.com/@zellwk/a-new-and-easy-way-to-hide-content-accessibly-92e21e159b85)
- [CSS in Action: Invisible Content Just for Screen Reader Users - WebAIM](https://webaim.org/techniques/css/invisiblecontent/)
- [HTML5 Accessibility Chops: hidden and aria-hidden - TPGi](https://webaim.org/techniques/css/invisiblecontent/)
- [Beware smushed off-screen accessible text - Medium](https://medium.com/@jessebeach/beware-smushed-off-screen-accessible-text-5952a4c2cbfe)
- [How to Hide Text from Screen Readers - PluralSight](https://www.pluralsight.com/guides/how-to-hide-text-from-screen-readers)
- [How to improve web accessibility by hiding elements - nomensa](https://www.nomensa.com/blog/how-improve-web-accessibility-hiding-elements)

### Alternative Text
- [Alternative text - WebAIM](https://webaim.org/techniques/css/invisiblecontent/)
- [How to Design Great Alt Text: An Introduction - deque](https://www.deque.com/blog/great-alt-text-introduction/)
- [Accessible Emoji's - dev](https://dev.to/finallynero/accessible-emojis--1pjh)

### Resources
- [WAVE Web Accessibility Evaluation Tool](https://wave.webaim.org/)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse/)
- [PurifyCSS Online](https://purifycss.online/)
---