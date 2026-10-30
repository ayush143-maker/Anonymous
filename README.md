# Anonymous

Anonymous is a single-page, terminal-styled chat demo with an ID/status header, message log, text field, and **SEND** button. Enter submits a nonblank message; the button sends it as well. Blank input is ignored.

## Messaging and presence

The page uses MQTT.js to connect to the public HiveMQ broker over WebSockets. It subscribes and publishes on `voidbox/m/v2` and `voidbox/p/v2`. This is a public-broker demo, not a private chat service.

Each browser session generates a random ID and broadcasts a presence heartbeat every four seconds. A user is considered stale after 12 seconds. The page holds messages and presence in in-memory Maps; when a user becomes stale, that user's messages are removed. This state is ephemeral: the entrypoint shows no persistent storage, and the app is not a persistent chat service.

## Open locally

No installation is required. Open `index.html` in a browser, or serve the repository with:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). The MQTT connection uses a public broker, so this demo should not be treated as private messaging.

## Customize

`index.html` is the page entry point and contains the visible interface and MQTT behavior. Keep any referenced assets at their existing relative paths, or update the references if files move. No framework or persistent storage is shown in the entrypoint.

## File reference

- `index.html` — page entry point and main location for content and behavior changes.