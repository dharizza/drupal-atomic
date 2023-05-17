# Drupal project for Atomic & Molecular Design training

In this project we're including a basic set of configuration for working on the Atomic & Molecular Design training.
The development environment configured for this project uses `ddev`, so make sure you install it by following the instructions defined in the [official documentation](https://ddev.readthedocs.io/en/stable/users/install/ddev-installation/) for your operating system.

### Setup Drupal project

1. Clone this repository in a new folder, for example for creating it in the `atomic2023` folder you can run `git clone git@github.com:dharizza/drupal-atomic.git atomic2023`
2. `cd` into your project's folder, for example with `cd atomic2023`
3. Run `ddev start`
5. Run `ddev composer install`
6. Run `ddev drush si --existing-config --account-pass=admin -y`

### Compiling theme

1. Make sure `nvm` is already installed in your system. This helps you manage
   multiple versions of Node JS.
2. Open the terminal and `cd` into your theme's directory, for example: `cd web/themes/custom/atomic_design`
3. Use the node version defined in the `.nvmrc` file in the theme directory. To do so run `nvm use`.
4. Install theme dependencies including `gulp`, libraries and other tools by running `npm install`.
5. Run `npm run gulp watch` to watch your SCSS / JS files for changes. When changes are detected, the respective CSS / JS files will be
   compiled and placed in the `css` and the `js` directories respectively.
6. To compile for production run `npm run gulp`
