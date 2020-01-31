# WPKit Theme + Webpack Instructions

WPKit Theme as version `2.1.0` now comes bundled with Webpack and starter ScSS and JS files.

```base
cd some/path/to/wp-content/themes/
composer create-project wp-kit/theme=2.* theme --prefer-dist
cd theme
npm i
npm start
```

Open the website in a browser and whenever you make changes to SCSS or JS files inside the `src` folder the browser will auto refresh

When you want to build for production:

```bash
npm run build
```

More information can be seen in respective repositories:

* WP Theme: https://github.com/wp-kit/theme
* Webpack: https://github.com/wp-kit/webpack
