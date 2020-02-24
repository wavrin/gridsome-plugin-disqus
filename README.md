# Disqus plugin for Gridsome

See [vue-disqus](https://github.com/ktquez/vue-disqus) for more options. And get your own Disqus shortname at their [site](https://disqus.com/).

## Install

- yarn add gridsome-plugin-disqus
- npm install gridsome-plugin-disqus

## Usage

Add the plugin to your `gridsome.config.js` file:

```js
module.exports = {
  plugins: [
    {
      use: "@gridsome/gridsome-plugin-disqus"
    }
  ]
};
```

Add a comments snippet to your article or blog template. Make sure you put your own Disqus "shortname" in it:

```html
<div class="post-comments">
  <vue-disqus
    shortname="DISQUSSHORTNAME"
    :identifier="$page.post.title"
  ></vue-disqus>
</div>
```
