# Instructions for developers in plugin development process

## NPM
* For development and gulp task we must be in root plugin folder and execute `$ npm install`
* For view npm version `$ npm -v`
* Update npm to latest version `$ npm install -g npm@latest`
* For update npm packages globally use `$ npm update -g`
* Folder ___node_modules___ isn't tracked in Git and we must update npm modules (previous step)
* We'll execute `$ npm audit` for view vulnerabilities problems and
* `$ npm audit fix` for fix them

## PHP Code Sniffer
* Whitelist phpcs errors:
  * https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards/wiki/Whitelisting-code-which-flags-errors
  * https://github.com/squizlabs/PHP_CodeSniffer/wiki/Advanced-Usage

## PhpCodeFixer
`$ phpcf directory` for check compatibility con PHP versions and problems, for install it:
1. Install composer:
`$ curl -sS https://getcomposer.org/installer | php`
2. Install phpcf in global composer dir:
`$ ./composer.phar global require wapmorgan/php-code-fixer dev-master`
3. Run from any folder:
`$ phpcf -h`
