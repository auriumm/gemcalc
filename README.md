# GemCalc

GemCalc is a small single-page tool for Hebrew text gematria analysis. The HTML page loads its own CSS and JavaScript from the local `styles/` and `scripts/` folders.

## Project layout
If you only saw one large HTML file before, the code is now split into three files so it is easier to read and maintain:

```
README.md
styles/
  gemcalc.css       # All styles
scripts/
  gemcalc.js        # All JavaScript
 gemcalc_fib_lucas_v1.html # HTML that links to the CSS/JS above
```

On GitHub (or any code host), you should see the `styles/` and `scripts/` folders next to the HTML file. Download or clone the repo as-is to keep that structure intact.

## Running without a server
You can open GemCalc directly from disk; no web server is required:

1. Download or unzip the project so the files stay together (keep `gemcalc_fib_lucas_v1.html`, `styles/gemcalc.css`, and `scripts/gemcalc.js` in the same folder structure).
2. Double-click `gemcalc_fib_lucas_v1.html` to open it in your browser. Modern browsers allow module scripts to load from the local filesystem, so the page will pull in the CSS and JS automatically.
3. You can use **Text mode** and **Search** immediately. **Verse mode** still needs an internet connection to reach the Sefaria API.

If you prefer, you can also serve the folder with a lightweight server (e.g., `python -m http.server 8000`), but it is not required just to test the app.
