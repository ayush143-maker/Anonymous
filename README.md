# Anonymous

A compact, terminal-inspired web experiment with a dark screen, green monospace text, a message log, and an input field. The page provides a front-end experience; it does not establish that input is sent to a chat service or that conversation history is saved.

## Open the page

No package installation is required. Open `index.html` in a browser, or serve the repository locally:

```sh
python -m http.server 8000
```

Visit [http://localhost:8000](http://localhost:8000). To host the page, serve `index.html` and any referenced assets together as static files.

## Personalize and review

The page is contained in `index.html`. Edit its visible text and presentation there. If you change or add asset references, keep the referenced files alongside the page at the corresponding relative paths; this repository lists no separate asset directory. Reload the page after editing and review the terminal-style contrast and layout, including at a narrow window width.