Theme used for atomic_design training. This theme was generated from starter kit_theme. Additional information on generating themes can be found in the [Starterkit documentation](https://www.drupal.org/docs/core-modules-and-themes/core-themes/starterkit-theme).

The theme generated with starter kit was updated to include a gulp setup, so we can compile Sass and JS.

Here's how you can get the ball rolling:

### One-time setup

1. Install `nvm` if it is not already installed. This helps you manage
   multiple versions of Node JS.

2. Open the terminal and `cd` into your theme's directory.

3. Use the node version defined in the `.nvmrc` file in this directory. To use the correct
   version of node for this project, simply `cd` into your theme's directory
   and run `nvm use`.

4. Next, we install `gulp`. Gulp will help us compile SASS / JS files. Simply
   run `npm install` and all the right tools and libraries will be installed.

### Compiling CSS / JS

First you have to install `nvm` and `gulp` as per instructions above. Once that
is done, you should be able to run `nvm --version`, you should be able to
see the respective version without any error.

Now whenever you want to work with SASS / JS, do the following:

1. Open a terminal window and `cd` into your theme's directory.

2. Run `nvm use` to make sure that you're using the right version of Node.

3. Run `npm run gulp watch` and it will watch your SCSS / JS files for changes. As
   and when changes are detected, the respective CSS / JS files will be
   compiled and placed in the `css` and the `js` directories respectively.

You can then test your CSS / JS changes and if you're happy with them, you can
commit them into the version control system.
