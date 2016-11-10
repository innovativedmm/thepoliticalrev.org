![The Political Revolution](assets/images/Bumper.png "The Political Revolution")[![Build Status](https://travis-ci.org/Smona/thepoliticalrev.org.svg?branch=master)](https://travis-ci.org/Smona/thepoliticalrev.org)

# Color Palette

Navy #04243E | Red #D34749 | Aqua #43C4DA | Cream #F9F9F9 | Olive #B9C3B7

# Deployment

## Development

Pushes to the master branch on GitHub will trigger a 
[Travis CI](https://travis-ci.org/Smona/thepoliticalrev.org) build. This will publish
the site on GitHub Pages, to <https://smona.github.io/thepoliticalrev.org>.

The Travis build script at `.travis.yml` installs node.js and rvm, and then runs the
`ci-deploy.sh` script.

`ci-deploy.sh` clones the repo into the `public_html` directory, runs `ci-compile.sh`
which compiles the JS files and HTML files using webpack and jekyll into that
directory, and then commits and pushes to the `gh-pages` branch. (This file is
well-commented, so most of the details are in the file itself.)

The script uses Travis CI encypted keys. For more info, see
<https://gist.github.com/domenic/ec8b0fc8ab45f39403dd>.

# Credits

Forty by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
