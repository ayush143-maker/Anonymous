# Anonymous

**Anonymous** is a compact, terminal-inspired web experiment. Its dark screen, green monospace text, and small input area give the page the feel of an old-school command console, while keeping the interaction simple and focused.

The current interface is built around a message log and an input/send control. This README describes the front-end experience only; it does not assume a connected chat service, saved conversation history, or a remote backend.

## Open the page

There is no package installation step for the current repository. Open the index.html file in a modern browser. For a local web server, run this from the repository directory:

    python -m http.server 8000

Then visit http://localhost:8000.

## Making changes

The page is self-contained in index.html. Keep the layout responsive and preserve the terminal-style contrast when adjusting typography, spacing, or interaction states. If a backend is added later, document its endpoint and setup separately rather than treating the current interface as a working messaging service.
