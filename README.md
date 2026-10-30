# Anonymous

A compact, terminal-inspired web experiment with a dark screen, green monospace text, a message log, and an input field. The page provides a front-end experience; it does not establish that input is sent to a chat service or that conversation history is saved.

## Open the page

No package installation is required. Open `index.html` in a browser, or serve the repository locally:

```sh
python -m http.server 8000
```

Visit [http://localhost:8000](http://localhost:8000). To host the page, serve `index.html` and any referenced assets together as static files.

## Personalize

The page is contained in `index.html`. Edit its visible text and presentation there. If you change or add asset references, keep the referenced files alongside the page at the corresponding relative paths; this repository lists no separate asset directory.

## Browser and layout review checklist

These are checks to perform, not verified results. No browser compatibility review is recorded here.

- [ ] Open the page in current versions of the browsers relevant to your audience. If an issue occurs, note the browser and version so it can be reproduced.
- [ ] Open the browser developer tools and inspect the Console and Network panel. Investigate JavaScript errors, failed requests, and other unexpected warnings; distinguish expected behavior from problems rather than assuming an empty console.
- [ ] Check every local asset reference in `index.html` against the files and paths in the repository. If you add remote resources, verify their URLs and check how the page appears when they are unavailable.
- [ ] Compare a narrow mobile-sized viewport with a desktop-sized viewport. Check that the message log and input remain visible, readable, and usable, and that resizing does not obscure content.
- [ ] Try the visible input and any other controls. Observe what the page actually does; do not assume input is sent to a service or saved.

## Accessibility review checklist

These are future checks, not compliance claims or verified results:

- [ ] Use Tab and Shift+Tab to reach the message input and other interactive controls. Check keyboard order and operation.
- [ ] Confirm focused controls have visible focus indicators against the dark, green presentation.
- [ ] Check that the input and controls have meaningful accessible names, not just placeholder text or visual styling.
- [ ] Check text and control contrast, including green text on the dark screen.
- [ ] If meaningful media is present or added, check its text alternatives; treat decorative media accordingly. If motion is present or added, check reduced-motion behavior.

No review results are recorded here; complete the checklists in a browser after making changes.