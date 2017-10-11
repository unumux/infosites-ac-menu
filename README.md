# willow-base
starting html for a willow-based website

## initial options

* theme-enterprise-default
* basic javascript to enable mobile nav toggle
* index page filled out with common options
* global-alert and secondary-nav commented out but exist in the html
* .gitignore augmented to ignore complied css and js .min
* html placeholder to avoid "missing favicon" error until you put one in

## Using this 
Make a folder, go into it and clone this into it:

    git clone https://github.com/townivan/willow-base.git .

Then disconnect your project from this repo: (delete hidden .git folder - example on a mac)

    rm -rf .git

Now you can run the UX command (say YES to all the prompts) to build up your site.

    ux

Then connect it to your own repo: 

!! [To avoid errors, do not initialize the new repository with README, license, or gitignore files](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/) !!

    git init



## Changing themes
If you want to use a different theme, it's as easy as:

Running either

    npm install --save-dev @unumux/theme-unum-default

or

    npm install --save-dev @unumux/theme-coloniallife-default

Then updating your styles/styles.scss file (at the top of the file) with:

    @import "node_modules/@unumux/theme-unum-default/styles";

or

    @import "node_modules/@unumux/theme-coloniallife-default/styles";
