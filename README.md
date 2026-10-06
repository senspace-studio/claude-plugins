# Claude plugins from Senspace Studio

A marketplace of Claude plugins. Each plugin lives under [plugins/](plugins/), and its README says how to connect it.

## Claude Code

Add the marketplace and install a plugin by name:

```
/plugin marketplace add senspace-studio/claude-plugins
/plugin install <plugin>@senspace
```

Update a plugin, then restart to apply it:

```
claude plugin update <plugin>@senspace
```

## Claude on the web and Desktop

Open "Customize", then "Plugins", add `senspace-studio/claude-plugins` as a marketplace, and install a plugin from it. Updates arrive on their own.
