# GitHub Pages website template for Debojjal Bagchi

Author:
Debojjal Bagchi
The University of Texas at Austin
debojjalb@utexas.edu
https://debojjalb@githiub.io

## Details

Based on the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

## Licensing 
The template is forked from ork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 

If you are forking this repository instead of the original repository please add credits to bpth original authors and me!


## To run locally (not on GitHub Pages, to serve on your own computer)
1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.
