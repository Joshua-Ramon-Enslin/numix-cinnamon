###Numix for cinnamon (white - blue fork)

####Notes on the fork
Below is the readme of the original numix-cinnamon theme. This is a fork aiming to keep the original look while making it lighter. Colors are replaced: dark grey with very light grey, lighter dark grey with a bit darker greys. On most occassions, red was replaced with blue. 
This fork is incomplete - it focuses on changes to the panel. E.g. the workspace switcher was not changed.

---

####Installation

Move the `Numix-Cinnamon` folder into your `~/.themes` directory.

---

####Compatibility

The latest version of this theme is on the master branch, and it supports cinnamon version `2.8`.

For older versions, check the available [releases](../../releases).

---

####Development

This theme is written using the css preprocessor [sass](http://sass-lang.com/).

You should use the provided `gulpfile.js` for improved workflow and speed!

---

__In order to use gulp:__

* Install [nodejs](https://nodejs.org/) and [npm](https://www.npmjs.com/).
    * If you want to contribute, make sure you run the nodejs version from the `.nvmrc` file! Use [Nvm!](https://github.com/creationix/nvm)

* Install [gulp](http://gulpjs.com/) globally:
    ```sh
    $ npm install --global gulp
    ```

* In the directory where the `gulpfile.js` file is, run:
    ```sh
    $ npm install
    ```

* In the same dir, run the following to use gulp:
    ```sh
    $ gulp
    ```

---

__Gulp will:__

* __Make a symlink of the__ `Numix-Cinnamon` __folder inside the__ `~/.themes` __dir.__

    * It will create a `~/.themes` dir if it doesn't exist already.

    * Even if you change the location of your working directory, running `gulp` will update the link.

    * If you already have a folder/file named `Numix-Cinnamon` in your `.themes` dir, it will be __deleted__.

* __Compile sass__ whenever certain files change.
    * Open `gulpfile.js` to see what files/folders are being watched.

* __Autoreload the theme.__
    * Under cinnamon, this will only work for changes in the (s)css files. When modifying images, you will have to restart cinnamon.
