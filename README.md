# WPKit Theme + ITCSS Instructions

* cd some/path/to/wp-content/themes/
* composer create-project wp-kit/theme=2.* theme --prefer-dist
* cd theme
* git clone https://github.com/wp-kit/itcss.git .
* npm i
* npm run build

Whenever you make changes to SCSS or JS files

* npm run build

Alterntively watch files and auto-build

* npm start

More information can be seen in respective repositories:

* WP Theme: https://github.com/wp-kit/theme
* ITCSS: https://github.com/wp-kit/itcss
