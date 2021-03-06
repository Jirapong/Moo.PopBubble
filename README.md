# Moo.PopBubble
A simple, light-weight contextual menu for links that supports buttons and forms.

# How to use
- Add `<script src="/[your-script-directory]/pop.js"></script>` to your HTML (remember to load MooTools 1.5.2 or higher *before* adding this tag).
- For simple text bubbles add `class="popBubble"` to your links and `data-pop-text` attribute with your message text (see *pop-sample.html*).
- For bubbles with a link button also add `data-pop-button` attribute with the text that you want to appear in your bubble's buttom (yes it does **support JavaScript functions**).
- For bubbles with simple input forms you will need:
  1. Have `class="popBubble"` and `data-pop-text` attribute in place within your links as well as `data-pop-form` attribute with an ID of your form (see demo.html)
  2. You will also need to actually create the form within your html with the same ID as in the `data-pop-form` attribute in your link. *Note that currently the script and CSS in this plugin (or app, if you wish) only supports simple forms with a single button and a single text-input field*

# Constructor
You can also dynamically create objects using `var myPop = new popBubble(element, options)` and call it via `myPop.pop(text)`, which adds a lot of power and is ridiculously easy to control.

The `options` can implement `styles: {}` object, where you can pass any CSS you wish, same way as if you'd pass it to any element using `MooTools.setStyles()` notation. It also has `offset: { x: 10, y: 20 }` that you can modify, as well as `text: text`, `button: text`, `action: [URL/JavaScript in text form]` and `form: [form element id]` that you could initialize with.

It really is easy to use and the best way to learn I find is by doing. So checkout demo.html for examples and explainations in comments.
