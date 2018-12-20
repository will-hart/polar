# Polar

A recipe for creating academic documents from Markdown using [pandemic](https://github.com/lionel-rigoux/pandemic)

## Installation

First make sure [pandemic](https://github.com/lionel-rigoux/pandemic) and all the standard filters are installed.

You will also need to install two more filters:

```bash
npm i -g pandemic-it-figures
npm i -g pandemic-mustache
```

Then install the `polar` recipe,

```bash
pandemic resource install recipe --as polar https://github.com/will-hart/polar.git
```

## Usage

Supply `polar` as the recipe either in the YAML front matter:

```yaml
pandemic:
  recipe: polar
```

Or by supplying the argument at the pandemic command line:

```bash
pandemic publish --to polar
```

## Purpose

`polar` is being used to help write chapters for my PhD thesis. Each chapter is a self-contained pandemic project. When building a `tex` file, these are included in a top level LaTeX template. A `node` script will be used to build all the chapters separately and then build the main document.
