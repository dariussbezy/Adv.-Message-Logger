# Adv. Message Logger

A Valenced beta that keeps a local, searchable journal of message edits and deletions observed by Discord on this device.

## Install

Add the following URL in **Valenced → Plugins → Advanced**, then install **Adv. Message Logger** from **beta**.

```text
https://raw.githubusercontent.com/dariussbezy/Adv.-Message-Logger/main/index.json
```

Version **1.0.0-beta** targets Discord **352.6** and Valenced Plugin API **1**.

## What this beta includes

- Native Discord settings, a searchable history and message details with **Jump to message** or **Open channel**.
- Separate edit and deletion switches, bulk deletion capture, filters for bots and self, and ignored server, channel or user IDs.
- Optional direct message alerts and optional local persistence. History stays in memory by default. You can clear the journal and recent snapshots in Settings.
- Optional cooperation with [Ghost Ping Logger](https://github.com/dariussbezy/Ghost-Ping-Logger). Both keep their own journals. When both would alert for the same event, Ghost Ping Logger handles the notification.

This beta shows logged text in the journal. It does not keep deleted rows in the chat or render edit history inline. It cannot recover messages the client never received and does not upload logs. Native mobile rendering still needs device testing.

## Development

Run `bun install --frozen-lockfile` and then `npm run publish:local` to build the ZIP and regenerate the index. Run `npm run lint:types` and `npm test` to check the build.
