# A Svelte Template with SASS Support

This Svelte app is based on the project template at [https://github.com/sveltejs/template](https://github.com/sveltejs/template), with the addition of SASS/SCSS support from [svelte-preprocess](https://github.com/kaisermann/svelte-preprocess).

It also should handle the other processors enabled by `svelte-preprocess`:

- pug
- coffeescript or coffee
- less
- scss or sass
- stylus
- postcss
- globalStyle (transform `<style global>` into global styles.)

## What to Change

You can clone this template with `degit dceddia/svelte-template-sass` or just make a few small changes to your own app. The changes are minimal:

- `npm install svelte-preprocess`
- Update `rollup.config.js` to add "preprocess" to the `svelte` plugin (you'll also need to import `autoPreprocess`)

```js
// add this import:
import autoPreprocess from 'svelte-preprocess';

// and inside the svelte plugin, add autoPreprocess:
export default {
  /* ... */
  plugins: [
    svelte({
      /* ... */
      preprocess: autoPreprocess()
  }),
  /* ... */
}
```
