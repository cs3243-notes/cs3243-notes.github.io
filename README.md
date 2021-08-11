These notes are based on CS 3243: Introduction to Artificial Intelligence taught by [Kuldeep S. Meel](https://www.comp.nus.edu.sg/~meel/) in Fall 2020 (Sem 1 of AY 20-21).

## Contributing

This material is still under construction! Although most of the notes have been written up in PDF format, you will probably find several typos. If you do, please inform us under GitHub issues or submit a pull request with your fixes via GitHub.

We are aiming to write our notes in Markdown, which will then be compiled into HTML using Jekyll. Please add your changes directly in Markdown source code.

To make any changes to this repo,

1. Fork this repo by clicking the "fork" button in the top right.
1. Make the changes you want and push them to your own forked copy of this repo.
   - The .md files for the lecture notes can be located under `/files/<lecture_name>.md`.
1. Go back to GitHub to creata a pull request to bring your changes into this repo.

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
   - Note that the latest version of ruby may not be compatible; ruby version 2.7 may be needed.
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

## Notes about writing math equations

- Start and end math equations with `$$` **for both inline and display equations**. To make a display equation, put one newline before the starting `$$` a newline after the ending `$$`.

- Avoid vertical bars `|` in any inline math equations (i.e., within a paragraph of text). Otherwise, the GitHub Markdown compiler will interpret it as a table cell element (see GitHub Markdown spec [here](https://github.github.com/gfm/)). Instead, use one of `\mid`, `\vert`, `\lvert`, or `\rvert` instead. For double bar lines, write `\|` instead of `||`.

## Acknowledgements

The handwritten notes were compiled into LaTeX by Priyanka Golia, with help from students including Ang Zheng Yong, Guo Yichao, Khiew Zhi Kai, and Vincent Neo.
