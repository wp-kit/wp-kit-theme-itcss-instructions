# WPKit Theme + ITCSS Instructions

```base
cd some/path/to/wp-content/themes/
composer create-project wp-kit/theme=2.* theme --prefer-dist
cd theme
git clone https://github.com/wp-kit/itcss.git tmp && rm -R tmp/.git && mv tmp/* . && rm -R tmp
npm i
npm run build
```

Update `theme/resources/AppController.php` with the following

__old__
```php
/**
 * @var array
 */
public $scripts = [
	'style.css',
];
```

__new__
```php
/**
 * @var array
 */
public $scripts = [
	'styles/style.css',
  	'scripts/application.min.js'
];
```

Whenever you make changes to SCSS or JS files

```bash
npm run build
```

Alterntively watch files and auto-build

```bash
npm start
```

More information can be seen in respective repositories:

* WP Theme: https://github.com/wp-kit/theme
* ITCSS: https://github.com/wp-kit/itcss
