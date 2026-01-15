# Genos IDE - Personal VS Code Fork

This is a personal fork of VS Code configured for **zero telemetry**.

## What's Different

| Feature | Microsoft VS Code | This Fork |
|---------|-------------------|-----------|
| Telemetry | Enabled by default | **Completely disabled** |
| Application Insights | Active | **Removed** |
| Copilot Integration | Built-in | **Removed** |
| Extension Gallery | Microsoft Marketplace | **Open VSX** |
| Branding | Visual Studio Code | **Genos IDE** |

## Telemetry Removal

The following telemetry components have been removed/disabled:

### product.json Changes

```json
{
  "enabledTelemetryLevels": {
    "error": false,
    "usage": false
  }
}
```

### Removed Sections

- `aiConfig` - No Application Insights key
- `defaultChatAgent` - No Copilot integration

## Keeping Updated

This fork tracks Microsoft's upstream:

```bash
# Add upstream (one time)
git remote add upstream https://github.com/microsoft/vscode.git

# Update from upstream
git fetch upstream
git merge upstream/main
git push origin main
```

## Building

See the main Genos IDE repository for build instructions:
`genos-ide/gama-dev-ide/vscodium-build/GENOS-VSCODE-FORK.md`

## License

MIT License - Same as VS Code
