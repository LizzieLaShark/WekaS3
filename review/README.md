# Review

Your HTML is good functionally for the most part, but formatting needs a lot of work.

In your stylesheet, make sure to indent the contents of each set of rules by two spaces. So this:

```css
h1.WebsiteTitle {
color: #6495ED;
background-color: yellow;
font-family: "comic sans";
font-size: 50px;
text-align: center;
}
```

Becomes this:

```css
h1.website-title {
  color: #6495ED;
  background-color: yellow;
  font-family: "comic sans";
  font-size: 50px;
  text-align: center;
}
```

Also, use "train-case" or "parameterization" (all lowercase and separated by hyphens) for CSS selectors (IDs and class names). So `website-title` not `WebsiteTitle`. There is some controversy about this, but the general consensus currently (unless you're using a namespaced system like BEM) is to use train-case. (Of course, you have to change it in the HTML attributes as well.)

Also, your paragraphs should be wrapped by *you*, not be automatic wrapping, at 80 characters or less. Yeah, I know it's a pain, but you won't be doing much of it. (Who makes static websites anymore?) It's a good habit to develop, and a large part of the benefit of coming to EDA is to develop good habits that you might not develop on your own.

I'm confused by some of your HTML. For example, you have one paragraph that has blank lines in it. Did you intend this to be multiple paragraphs? Do you understand that HTML collapses whitespace? So you cannot create paragraphs (or anything else) by adding more spacing. You have to use `<p>` elements to create paragraphs.

When you get a chance, maybe ping me on Slack if you need more explanation.

Your indentation is also wrong. Two spaces, please, not three.

Great use of HTML character entities (`&amp;`)! You might be the only one of your classmates using them. Nice work.

On the JavaScript, your cube is good, but the parentheses are unnecessary. You don't need to group the operations because it doesn't matter what order they are done in. `x * x * x` is the same as `(x * x) * x` is the same as `x * (x * x)`.

What happened to the other functions?

Also, please follow the style guide [standard.js rules](http://standardjs.com/rules.html). Operators have spaces around them:

```js
function cube (x) {
  return x * x * x
}
```

Very good observations on POUR and on responsive vs. native apps. I never really thought about it this way before, but I think you're right: native apps are a bit elitist. Not to mention more expensive to make. (And websites are usually free, but apps often cost something. Hmm.)

What happened to your user needs and product objectives? Ping me on Slack if you need help.

