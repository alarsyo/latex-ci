# Automated LaTeX document build

This is a proof of concept for automatically building and publishing (and
sharing with uninitiated users) a LaTeX document with GitHub Actions.

To use this in your repo, simply copy
[`.github/workflows/build-doc.yaml`](./.github/workflows/build-doc.yaml) to your
repo, keeping the same file path, and tweak the file names such as `doc.tex` and
`doc.pdf`.

The document is built on each commit push and is available as a build artifact
(see https://github.com/alarsyo/latex-ci/actions), however artifacts are only
downloadable as zip files.

For direct access to the PDF file, one can create a tagged release ([see this SO
answer for how to do it in a few clicks from
GitHub](https://stackoverflow.com/a/18223354)) and the GitHub Action will
automatically attach the PDF file to that release.
