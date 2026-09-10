# Math Slides — Linear Equations

A small HTML presentation with **remark.js slides and MathJax notation**, showing worked solutions to two linear equations. The slide content is in Spanish; this guide is in English.

## Run locally

From the repository root, use Python 3 to start a static server:

```sh
python -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000` in a browser. No npm installation or build step is required to view the checked-in example. Stop the server with `Ctrl+C`.

## Content and editing

The deck contains a title slide and worked examples for `5x + 4 = 1 - x` and `-3x + 5x/9 = 4/3 - 2x`. Their final values are `x = -1/2` and `x = -3`.

Edit the Markdown/HTML inside `<textarea id="source">` in [index.html](index.html). A `---` line separates slides. Math expressions use TeX delimiters, and [styles.css](styles.css) controls layout and emphasis.

The page loads remark.js, MathJax, and a legacy polyfill script from external hosts, so a local server alone does not make it work offline. Review external script dependencies before publishing a maintained version.

## Original previews

The original screenshots are externally hosted historical references. Their availability is not guaranteed:

- [Title slide](https://pbs.twimg.com/media/EhnIGO7WkAEruOu?format=jpg&name=medium)
- [First worked example](https://pbs.twimg.com/media/EhnIJi6X0AElU9y?format=jpg&name=medium)
- [Second worked example](https://pbs.twimg.com/media/EhnIQFHWAAAxnQv?format=jpg&name=medium)

## Verification and known issues

There is no automated test suite. Check that the slide viewer loads, equations are typeset, and slide navigation works before presenting. The second example contains an intermediate line missing an `x` and explanatory text that does not match the displayed operations; review these steps before teaching from the deck. This documentation update does not change the mathematical slide source.
