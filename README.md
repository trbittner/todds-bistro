* Styles for the recipe cards used from [here](http://freefrontend.com/css-cards/#recipe-cards).
* The storage location for [our images](https://postimages.org/).
* [Gravit](https://designer.gravit.io/) is a browser based alternative to Inkscape.
* [This](https://fonts.google.com/specimen/Shadows+Into+Light) is likely the font for our front page.
* The [inspiration](https://codepen.io/amwill/pen/YyexrJ) for the style of our front page.
* Notes on CSS positioning [here](https://www.w3schools.com/cssref/pr_class_position.asp).
* The best way to figure out [box shadows](https://www.w3schools.com/cssref/css3_pr_box-shadow.asp) 
in CSS is [to play](https://www.w3schools.com/cssref/tryit.asp?filename=trycss3_box-shadow) with them.
* [This styling](https://www.w3schools.com/css/css3_multiple_columns.asp) may prove useful for multiple columns when we need it.
* [Vue Router](https://router.vuejs.org/en/essentials/getting-started.html).
* [...and here's the link to the Vue guide itself](https://vuejs.org/v2/guide/single-file-components.html).

* Upgrading node with `nvm` is simple (note it's `nvm` not `npm`) - `nvm install stable`
* Then upgrade npm - `npm install npm@latest -g`

* Vue seems to be a bit heavy handed, but I don't want code duplication, so I'm going to try Google's 
[Firebase](https://firebase.google.com/).
* When logging in, use `firebase login --no-localhost`

* While researching firebase, I came across more information on static site generators.  I'm trying my hand at 
[gitlab pages](https://about.gitlab.com/features/pages/), specifically the [jekyll](https://gitlab.com/pages/jekyll) set up.
* `sudo apt-get update`
* `sudo apt-get install ruby` This is an old version of ruby, so we need to do some more work.
* `sudo apt-get install gnupg2`
* Follow [these instructions](http://rvm.io/) and [these hints](https://tecadmin.net/install-ruby-on-rails-on-ubuntu/).
* `sudo usermod -a -G rvm cabox`
* `rvm list known`
* `rvm install 2.4.1`
* `rvm use 2.4.1 --default`
* `sudo gem install jekyll bundler`
* [More information on using jekyll](http://damonbauer.me/organizing-jekyll-pages/).
* [Information on jekyll collections](https://learn.cloudcannon.com/jekyll/introduction-to-jekyll-collections/).
* There are [other filters](https://help.shopify.com/themes/liquid/filters/string-filters#capitalize) that are available, that aren't
mentioned in the jekyll documentation.
* [What the hell is a clearfix hack?](https://www.w3schools.com/howto/howto_css_clearfix.asp)
* [This site assisted me with layout inheritance](https://learn.cloudcannon.com/jekyll/introduction-to-jekyll-layouts/).
* [This](http://app.xrespond.com/) can be used for responsive testing.
* We use [this](https://designer.gravit.io/) for scanning and manipulating the drawings.
* [`margin: 0 auto`](https://stackoverflow.com/questions/3170772/what-does-auto-do-in-margin0-auto) explained.
* [This page](https://getbootstrap.com/docs/4.0/layout/overview/) gives @media queries for various breakpoint sizes.
* We'll likely use [this](https://codepen.io/nicokoenig/pen/jGmGvV) for cooking classes.  It's from the 
[same site](http://freefrontend.com/css-cards/#stacked-cards) we used for the recipe css.
* Not that it's necessary, but here are alternatives to 
[image storage](https://www.makeuseof.com/tag/4-imgur-alternatives-for-uploading-sharing-images/)
* From the scss file (re imports) - The @import rule must be at the top of the document (but after any @charset declaration).
* From the scss file (re gradients) - This indicates that from 0 - 24px on the gradient, transition from yellow to yellow (so, no transition).
From 24 - 25px transition from yellow to blue (essentially creating thin blue lines).
* [YAML cheat sheet | https://learn-the-web.algonquindesign.ca/topics/markdown-yaml-cheat-sheet/]