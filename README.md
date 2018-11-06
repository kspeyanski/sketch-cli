# How to run it?

Host a demo app locally, and pass the url to the script with `--url`.
Pass a second parameter being the output dir with `--out-dir`.

The script is located in `bin/cli.js`.

```sh
node bin/cli.js --url http://localhost:3000/examples/calendar/basic.html --out-dir dist
```

An example app has been made in the `kendo-react-private` repo, branch `sketch-test`, in `packages/dateinputs/examples/calendar/basic` just for a quick testing.

## Import to sketch

1. Open Sketch.
1. Click on `Plugins` in the top menu.
1. Click `From *Almost* Sketch to Sketch`.
1. Navigate to the `--out-dir` parameter.
1. Select the 2 `.json` files and click `choose`.
1. The Symbols should be loaded.

## Side Note
An `data-sketch-symbol` parameter should be set to the most wrapping element of our components. 
```html
<div data-sketch-symbol="MySymbol">
```

I has been added to the `Buttons/Calendar/Grid/Chart/ConversationalUI` components in the `sketch-test` branch of the `kendo-react-private`. This is the entry point for the `html-sketchapp` to start generating symbols.

## Whats different than the original repo?

The `generateAlmostSketch.js` file has been slightly modified to gather all styles from an element.