# ESOFacts

An Elder Scrolls Online addon that lets you share random lore facts with other players in chat.

## Features

- **56 lore facts** covering races, Daedric Princes, history, creatures, artifacts, and more
- **No-repeat system** - cycles through all facts before repeating
- **Cooldown** - 5-second cooldown prevents spam
- **Channel selection** - choose where to send facts
- **Auto mode** - automatically send facts on a timer (guild/group only)
- **Saved settings** - your channel preference and fact history persist between sessions
- **Keybind support** - bind a key to share facts (Settings > Keybindings > ESO Facts)

## Commands

| Command | Description |
|---------|-------------|
| `/facts` | Share a random fact (opens chat input ready to send) |
| `/factschannel` | Show current channel and available options |
| `/factschannel <channel>` | Set the output channel |
| `/factsauto <minutes>` | Start auto-sending facts at an interval |
| `/factstop` | Stop auto mode |

### Channel Options

- `say` - Local /say chat (default)
- `yell` - /yell chat
- `zone` - Zone chat
- `group` or `party` - Group/party chat
- `guild1` through `guild5` - Guild chats

## Keybind

You can bind a key to share facts instead of typing `/facts`:

1. Open Settings > Keybindings
2. Scroll to "ESO Facts"
3. Set your preferred key for "Share Random Fact"

## Auto Mode

Automatically sends facts to chat at a set interval. Includes safeguards to prevent spam:

- **Minimum interval**: 5 minutes
- **Maximum facts**: 10 (then auto-stops)
- **Restricted channels**: Only works with group and guild chat (not say, yell, or zone)

### Example Usage

```
/factschannel guild1
/factsauto 10
```

This sends a random fact to guild 1 every 10 minutes, stopping after 10 facts.

## Installation

1. Download and extract to your AddOns folder:
   - Windows: `Documents\Elder Scrolls Online\live\AddOns\ESOFacts`
2. Enable the addon in the game's addon menu
3. Type `/facts` in chat to get started

## License

MIT
