# HelpPlugin

**Version:** 1.0.0  
**Author:** herbs.acab  
**Description:** Displays a list of server features and commands when /help is typed.

## Features

- Provides a welcome message and a list of server commands when players type `/help` in chat.
- Allows admins to customize the welcome message and the list of commands through a data file.
- Supports message formatting and adding new lines.
- Console command to reload the plugin data without restarting the server.

## Installation

1. Download the `HelpPlugin.cs` file and place it in your `oxide/plugins` directory.
2. Start or restart your Rust server to load the plugin.
3. The plugin will create a data file in the `oxide/data` directory named `HelpPluginData.json`.

## Commands

### Chat Command

- **/help**
  - Displays the welcome message and a list of server commands.

### Console Command

- **helpplugin.reload**
  - Reloads the plugin data from the data file. Use this command after making changes to the data file.

## Configuration

The plugin uses a data file for configuration, located at `oxide/data/HelpPluginData.json`. This file allows admins to customize the welcome message and the list of commands.

### Editing the Data File

1. Open the `HelpPluginData.json` file in a text editor.
2. Modify the `WelcomeMessage` to change the welcome message displayed to players.
3. Modify the `Commands` array to change the list of commands displayed to players.
4. Save the file and use the `helpplugin.reload` console command to apply the changes.

### Example Welcome Message

- **Default Welcome Message:** `Welcome to [color=blue]Rusty Reef[/color]! Below is a list of commands that you can use, be sure to join our discord for announcements and support.`

### Example Commands

- **Default Commands:**
- `" - - - - - - - - - - - - - - - ",`
- `"/help - Display this help message",`
- `"/stats - Check your in-game stats",`
- `"/lookup playername - Check out someone's stats",`
- `"/clan - Manage your team",`
- `"/luckybox - Display the status of the luckybox",`
- `"- - - - - - - - - - - - - - - - "`
  
---

**Note:** The example above shows default values. Admins can customize these messages and commands as needed. I made this plugin for my server RustyReef, so it's default messages are for that.
