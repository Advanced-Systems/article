<p align="center">
  <a title="Project Logo">
    <img height="150" style="margin-top:15px" src="https://raw.githubusercontent.com/Advanced-Systems/vector-assets/master/advanced-systems-logo-annotated.svg">
  </a>
</p>

<h1 align="center">Advanced Systems Article Template</h1>

## About

This is a template repository for comprehensive LaTeX documents using the `article`
class. It features a glossary for acronyms and a bibliography. Additionally, the
sample sections *Introduction* and *Formulas* also provide code snippets for
embedding images, using tables or writing equations.

## Customize

Edit title, author and logo in `src/document.tex`. This template is broken down
into sections. Similarly, you may also make changes
to the following lines:

- `src/sections/`
- `src/acronyms.tex`
- `src/bibliography.bib`

## Compile

This example uses Advanced Systems' [Math Macros](https://github.com/Advanced-Systems/mathmacros);
while this package is in development, it is recommended to pull it in as a git submodule:

```cli
git submodule update --init --recursive
```

Both TeX Live and MikTeX come with `latexmk`, though since this is a
perl script you need to have perl installed on your system to run
this command. Alternatively, use the `pdflatex` command.

```cli
latexmk src/document.tex -outdir=build -pdf
```

## Clear Cache

```cli
latexmk -C -outdir=build
```
