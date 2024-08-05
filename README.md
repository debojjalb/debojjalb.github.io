# Github Pages Personal Website

**Author:**<br>
Debojjal Bagchi<br>
The University of Texas at Austin<br>
debojjalb@utexas.edu<br>
[https://debojjalb.github.io](https://debojjalb.github.io)

## Details

Based on the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

## Licensing

This template is forked from [this repository](https://github.com/academicpages/academicpages.github.io), with all rights belonging to the original authors. The current repository includes several modifications made by the author. Both the original content and the modifications are covered under the MIT License. See the [license file](LICENSE) for more details. 

If you choose to fork this repository rather than the original one, please credit both the original authors and myself.


## To run locally (not on GitHub Pages, to serve on your own computer)
1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.
