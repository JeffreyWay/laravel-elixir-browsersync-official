# Laravel Elixir Browsersync Support

This extension brings Browsersync support to Laravel Elixir version 6 and up. Prior to that release, Browsersync was baked in.

## Step 1: Install

```bash
npm install laravel-elixir-browsersync-official --save-dev
```

## Step 2: Use It

Within your Gulpfile, add:

```js
elixir(function(mix) {
  mix.browserSync();
});
```

Once you run `gulp watch`, access your web application using port 3000 to enable browser syncing: `http://homestead.app:3000`. 
If you're using a domain other than `homestead.app` for local development (likely), you may pass an array of options as the first argument to the browserSync method:

```js
elixir(function(mix) {
  mix.browserSync({
    proxy: 'project.app'
  });
});
```
