---
title: JavaScript - "Hello World"
date: "2019-07-02"
template: "post"
draft: false
slug: "/javascript/hello-world/"
category: "JavaScript"
tags:
  - "JavaScript"
  - "Web Development"
description: "In short, it goes from top to bottom, hence if script tags are at the bottom, JavaScript assumes document tree (whole HTML code) is loaded up and ready."
---

I am Starting with part of Core JavaScript, the language itself.

To run our scripts, of course, we need a working environment, so the browser is a good choice for now.

# **The "Script" tag**

JavaScript can be inserted into any part of an HTML document with the help of `<script>` tag. Script tag should be inside `<body>` tag and its better to put at end of the HTML file to ensure it (the page? or the JavaScript? or both?) loads quickly. In short, it goes from top to bottom, hence if script tags are at the bottom, JavaScript assumes document tree (whole HTML code) is loaded up and ready.

### _For instance :-_

```html
<!DOCTYPE html>
<html>
  <body>
    <p>Before the script...</p>

    <script>
      alert("Hello, world!");
    </script>
  </body>
</html>
```

Nowadays `<script>` tag is rarely used but still can found in old code.

## The “type” attribute: `<script type=”….”>`

The old HTML requires a script to have “type” it was type=”text/javascript” . We don’t need it anymore in HTML5 the modern HTML.

# **External Scripts**

Sometimes in big projects, it happens that you have a lot of JavaScript code, we put it into a separate file.

Script files are attached to HTML with the src attribute:-

```js
<script src="/path/script.js">// lines of code....</script>
```

Here, “/path/script.js” is an absolute path to the script file.

If you are using the external script, then you can’t have both the src attribute and code inside single `<script>`

```js
<script src="file.js">
  alert(1); // this content is ignored, because src is set
</script>
```
