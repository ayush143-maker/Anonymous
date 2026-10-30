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

## Manual review checklist

These are actions to perform, not verified results:

- [ ] Open `index.html` in a browser, or start the local server above and open its address.
- [ ] Check the page for missing images or other media. If you change or add references, verify that each path points to a file in the expected location.
- [ ] Try the visible input and any other controls. Check what the page actually does; do not assume input is sent to a service or saved.
- [ ] Inspect the terminal-style text, contrast, and layout at both narrow and wide window widths.

## Accessibility review checklist

These are future checks to perform, not compliance claims or verified results:

- [ ] Use Tab and Shift+Tab to reach the message input and any other interactive controls; check that keyboard order follows the page and that keyboard users can operate each control.
- [ ] While tabbing, confirm the focused control has a visible focus indicator against the dark, green terminal-style presentation.
- [ ] Check that the input and any controls have meaningful accessible names, not just placeholder text or visual styling.
- [ ] Check text and control contrast against their backgrounds, including the green text on the dark screen.
- [ ] If images or other meaningful media are present or added, check that they have appropriate text alternatives; treat purely decorative media accordingly.
- [ ] If motion or animated effects are present or added, check that they respect the operating system's reduced-motion preference.

No review results are recorded here; complete the checklists in the browser after making changes.