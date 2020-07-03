# Flexbox and Templating

---

# Mustache.js
- js templetting library
- ease to seperate data from presentation
- allow to write code easier to understand, maintain and extend

### Code Examples

- snippits.js => small pieces of javaScript code
- index.html => an example of a webpage
- style.css => for presentatoin only
- mustache-logo.png => for presentatoin only
`to use it, it should be included to the webpage`


#### Install `$ npm install mustache --save`

#### Usage
  `title: "Joe",
  calc: function () {
    return 2 + 4;
  }
};`
`var output = Mustache.render("{{title}} spends {{calc}}", view`
*Templates There are several techniques that can be used to load templates and hand them to mustache.js:*

  `<body onload="renderHello()">
    <div id="target">Loading...</div>
    <script id="template" type="x-tmpl-mustache">
      Hello {{ name }}!
    </script>`

    `<script src="https://unpkg.com/mustache@latest"></script>`
    `<script src="render.js"></script>`
  </body>
</html>`

- Include Templates
  `var template = document.getElementById('template').innerHTML;
  var rendered = Mustache.render(template, { name: 'Luke' });
  document.getElementById('target').innerHTML = rendered;}`

- Load External Templates using fetch :
`fetch('template.mustache')
 .then((response) => response.text())
 .then((template) => {
   var rendered = Mustache.render(template, { name: 'Luke' });
   document.getElementById('target').innerHTML = rendered;
 });
}`
- Learn Handlebars in 10 Minutes or Less
- What is Handlebars?
- Handlebars is a simple templating language

- A handlebars expression is a {{, some contents, followed by a }}. When the template is executed, these expressions are replaced with values from an input object.
- popular templating engine.
- based on the Mustache template language.
- Handlebars, able you to separate the generation of HTML from the rest of your JavaScript and write cleaner code.
- TryHandlebars (try it)
- Adding it to your project (try it)
- CDN's (try it)

---

### Templates
- They can contain HTML and text, mixed with Handlebars expressions.
- Expressions are wrapped in double or triple curly braces {{}}
- Templates need to be compiled to a JavaScript function before use.
- Expressions
- any data that you print out in an {{ }} expression, will automatically get HTML escaped by handlebars
- Context
*the object where properties you include in curly braces are looked up JavaScript object that pass to the compiled template. <script `id="example-template" type="text/x-handlebars-template">`*
- Helpers
- JavaScript functions that you can call from your templates, and help you reuse code and create complex templates.
- To call a helper, just use it as an expression - {{helpername}}.
- registerHelper function
- Block helpers
- have an opening and a closing tag (like the #if and #each built-ins)
- Handlebars.js vs Mustache
- Handlebars.js vs Mustache

- Handlebars.js vs Mustache: What are the differences?

- Handlebars.js:

- Minimal Templating on Steroids.
- Handlebars.js is an extension to the Mustache templating language created by Chris Wanstrath.
- Handlebars.js and Mustache are both logicless templating languages that keep the view and the code separated like we all know they should be;
- Mustache: Logic-less templates.

- Mustache is a logic-less template syntax.
- It can be used for HTML, config files, source code - anything.
- It works by expanding tags in a template using values provided in a hash or object.
- We call it "logic-less" because there are no if statements, else clauses, or** for loops**.
- Instead there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
- Handlebars.js and Mustache belong to "Templating Languages & Extensions" category of the tech stack.

- "Simple" is the top reason why over 102 developers like Handlebars.js, while over 29 developers mention "Dead simple templating" as the leading cause for choosing Mustache.

- Handlebars.js and Mustache are both open source tools. Handlebars.js with 14.5K GitHub stars and 1.86K forks on GitHub appears to be more popular than Mustache with 13.1K GitHub stars and 2.3K GitHub forks.

- Handlebars.js vs Mustache

- Handlebars.js vs Mustache

- A Complete Guide to Flexbox
- A Guide to Flexbox Flexbox Froggy

- display: flex; then the following will be written:
- justify-content property, which aligns items horizontally and accepts the following values:
- flex-start: Items align to the left side of the container.
- flex-end: Items align to the right side of the container.
- center: Items align at the center of the container.
- space-between: Items display with equal spacing between them.
- space-around: Items display with equal spacing around them.