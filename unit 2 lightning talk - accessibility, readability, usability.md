### Principles of Web Design - Accessibility, Readability, Usability

By: Lux Barker (they/them)

---

##### The Agenda

- define accessibility, readability, and usability as they relate to web design
- discuss why accessibility is important
- provide examples of common accessibility issues
- provide resources for learning more

---

##### Definitions

- **accessibility** --> an accessible website is a site that is usable, readable, and understandable by everyone regardless of ability or disability
- **usability** --> one aspect of accessibility
    - think user-centered design
    - consider: availability of the site, clarity of the information, learnability of the interface, credibility of the organization (or you!), and relevancy of the content
- **readability** --> another aspect of accessibility
    - consider: reading ease, hierarchical information architecture, contrast, typography

---

##### A Few Other Important Definitions

- **universal design** --> a design that is usable by everyone by default
- **equivalent use** --> accessible alternatives are provided that contain the same level of information as the "mainstream" version
- **accommodation** --> a separate "accessible" version of the content is provided but it does not hold the same amount or same kind of information as the "mainstream" version does
- universal design > equivalent use > accommodation
    - but of course, it's not actually that simple and often you need a combination of techniques!

---

##### Why is Accessibility Important?

- everybody has different needs and different ways of engaging with content
- without an emphasis on accessibility from the very beginning of a project throughout its entire lifetime, you can end up accidentally alienating a lot of folks who might have otherwise gained value or enjoyment from your project or product!
- *everyone* and *anyone* working on a web project should be thinking about accessibility; the role shouldn't be relegated to just one "accessibility cop"!

---

##### Common Accessibility Issues And Fixes

- low contrast text
    - presents a barrier for color-blind users
    - the fix: use a [color contrast checker](https://webaim.org/resources/contrastchecker/)
- missing alt text on images
    - presents a barrier for blind users
    - the fix: simply add alt text to all images with HTML!
- missing link text
    - for example: if just an image or button is used for a link with no textual description of what the link is to other than its URL
    - presents a barrier for users using a screenreader
    - the fix: add link text with an `<a>` tag in HTML, or possible alt text if you are using an image as a link!
- ambiguous link text like 'click here'
    - presents a barrier for users using a screenreader
    - the fix: use descriptive link text instead
- these are just a few of many common issues!

---

##### Learn More

- [Readability in design: principles of usability](https://readable.com/blog/readability-in-design-principles-of-usability/)
- [5 Key Principles of Good Website Usability](https://www.crazyegg.com/blog/principles-website-usability/)
- [Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [Top 8 Most Common Accessibility Issues to Avoid and Solve](https://www.accessiblemetrics.com/blog/top-8-most-common-accessibility-issues-to-avoid-and-solve/)
- [Web Content Accessibility Guidelines](https://www.w3.org/WAI/standards-guidelines/wcag/)
- [Web Accessibility Evaluation Tool](https://wave.webaim.org)