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

## Deployment-readiness checklist

These are actions to complete before and after publishing, not evidence that a deployment exists or that any checks have passed.

- [ ] Use the repository root as the page's source directory: it contains `index.html`. Make sure the published site root serves that file as its entry page. No separate build output directory or build script is listed for this repository.
- [ ] Check `index.html` for local asset references. Include every referenced file at the same relative path in the published files; if a path or file changes, update the reference and verify it locally.
- [ ] No `.env.example` or other configuration template is listed. Do not invent environment variables or add credentials to the HTML or other tracked files. Browser-delivered values are visible to visitors.
- [ ] Before publishing, open the page locally and check the visible content and controls. The input's appearance does not establish that it sends or saves messages.
- [ ] After publishing, open the published page in a browser. Confirm that `index.html` loads, the page renders as expected, and any referenced local assets load. Check the browser Console and Network panel for errors or failed requests.
- [ ] Review the published page at narrow and desktop-sized viewports, and try the visible input and other controls. Confirm their observed behavior rather than assuming a service or data handling.

## Contributor handoff

Keep a change focused on the intended page or asset. Preserve existing filenames and relative references unless a rename or move is necessary, and update references in `index.html` if paths change. In your handoff, summarize what changed and which files were affected. Manually review the page before publishing; the checklist above describes checks to perform, not results already verified.

## Troubleshooting

Use these as diagnostic steps; they are not reports of known problems.

1. Confirm that you opened this repository's `index.html`.
2. If the page or an asset is missing, check that any referenced local file exists at the path used in `index.html`. Preserve relative paths when moving files, or update the references.
3. Open the browser developer tools and inspect the Console and Network panel for errors and failed requests. A failed local-file request differs from an unavailable remote resource; check the request URL before deciding what to change. No external resources are listed for this page in the repository overview.

## Configuration and data handling

The listed repository files do not include an `.env.example` or separate configuration file. Do not add real credentials or private data to `index.html` or other tracked files. This page is delivered to visitors' browsers, so any value included in its HTML, scripts, or browser requests is visible and cannot be kept secret. If you add a configuration template, use placeholders rather than real values and document its purpose without publishing credentials. Do not assume the input is transmitted or saved; avoid entering real personal or sensitive information unless you have verified where it goes and how it is handled.

## Browser and layout review checklist

These are checks to perform, not verified results. No browser compatibility review is recorded here.

- [ ] Open the page in current versions of the browsers relevant to your audience. If an issue occurs, note the browser and version so it can be reproduced.
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

## Final release review

- Open `index.html` from the published location and confirm the page loads as expected.
- Review the published result once on a narrow screen and once on a wider screen; treat this as a release check, not an automated test report.
