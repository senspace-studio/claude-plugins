# Intelligence

Work from your company's records: search across every source, see how its accounts and posts are doing outside, and ground what Claude writes in what the records say, citing where each fact is written. The plugin is the intelligence MCP server, authenticated with a passphrase set by whoever runs the server, together with skills that use it. Other connectors it needs are listed in [CONNECTORS.md](CONNECTORS.md).

## Skills

Skills run when your request matches what they do, or by name, for example `/intelligence:update-from-records`. Each one is described in [skills/](skills/).

- `update-from-records`: writes into a table people keep by hand, such as a tracker, a guest list or a status sheet, the facts the records state. Every value carries its source, and nothing is written until you approve it.

## Install

In Claude Code, run:

```
/plugin marketplace add senspace-studio/claude-plugins
/plugin install intelligence@senspace
```

In Claude on the web and Desktop, open "Customize", then "Plugins", add `senspace-studio/claude-plugins` as a marketplace, and install `intelligence`.

After installing, open the intelligence connector, connect, and enter the passphrase on the page that opens.
