# Anonymous

A compact, terminal-inspired web experiment with a dark screen, green monospace text, a message log, and an input field. This is a front-end page; the presence of an input does not establish that messages are sent to a chat service or saved.

## Open locally

No installation is required. Open `index.html` in a browser, or serve the repository with:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). To host the page, serve `index.html` and its referenced assets together as static files.

## Customize

The page’s text and presentation are in `index.html`. Keep any referenced assets at their existing relative paths, or update the references if files move. No separate asset directory is listed for this repository.

## File reference

- `index.html` — page entry point and main location for content and presentation changes.

The repository does not document a build step or a connected messaging backend. Review the visible input’s actual behavior rather than assuming it transmits or retains data.