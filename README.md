# Custom CSS Themes for Joplin
[Joplin](https://joplinapp.org/) is an open-source markdown notetaking app. I've mostly used joplin for journaling and notetaking, so this is a collection of CSS themes that I've created to optimize my workflow and make Joplin more visually appealing.

Joplin's appearance can be customized with CSS coming from two files: `userstyle.css` and `userchrome.css`. `userstyle.css` controls the rendered markdown in the viewer and HTML/PDF exports. `userchrome.css` controls the the editor and overall app styles. These CSS customizations override existing Joplin styles, so you can add as little or as much as you want.

To use any of these themes just copy them into the Joplin-Desktop directory and change the file name to `userstyle.css` or `userchrome.css` corresponding to the style type.

**CONTENTS**

- userstyle.css Themes
	+ Custom HTML Tags
	+ Theme Previews
	
- userchrome.css Themes

- Installation / How To use
---


# userstyle.css
## Custom HTML Tags
Markdown supports HTML tags using `<>` brackets, so I've added support for various custom tags:

### Redact
The `<redact>` tag will redact the enclosed text and make it unreadable. The `reason` attribute can be used to display a message before the redacted text.
![Redact demo](./assets/HTML-redact-demo.png)

### Spoiler
Spoiler is a subclass of `redact`. The text will still be hidden at first, but if you hover over it the text will reveal itself. Similarly to the `reason` attribute, the `warning` attribute can be used to give a content warning to your spoilered text.
![Spoiler demo](.\assets\HTML-Spoiler-Demo.gif)