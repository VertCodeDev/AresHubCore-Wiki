<p align="center">
    <img height="128" src="https://cdn.vertcodedevelopment.com/logo.png" width="128" alt="VCD-Logo"/>
</p>
<h1 align="center">AresHubCore</h1>
<p align="center">A unique hub core plugin.</p>

## Features

- [x] Customizable items
- [x] Customizable menus
- [x] Customizable messages
- [x] Spawn System
- [x] Grief Protection
- [x] Parkour System
- [x] PVP Mode
- [x] Welcome System

## Commands

- `/ahc` - Main command
- `/ahc help` - Help command
- `/ahc setspawn` - Set the spawn location
- `/ahc spawn` - Teleports you to the spawn location
- `/ahc togglebuild <player>` - Toggle build mode for the provided player, only runnable by console.

## Permissions

- `ahc.*` - Gives access to all commands
- `ahc.command.help` - Gives access to the help command
- `ahc.command.setspawn` - Gives access to the setspawn command

## Configurations

**menus/example1.yml**

```yaml
title: '&6Example Menu'
layout:
  - [ '-', '-', '-', '-', '-', '-', '-', '-', '-' ]
  - [ '-', 'a', '-', 'b', '-', 'c', '-', 'd', '-' ]
  - [ '-', '-', '-', '-', '-', '-', '-', '-', '-' ]
items:
  filler:
    material: 'GRAY_STAINED_GLASS_PANE'
    icon: '-'
    display-name: '&7'
    lore: [ ]
  example1:
    material: 'DIAMOND_SWORD'
    icon: 'a'
    display-name: '&6Example Item 1'
    action:
      type: 'COMMAND'
      value: 'say Example Item 1'
      close-menu: true
    lore:
      - '&7This is an example item.'
  example2:
    material: 'DIAMOND_SWORD'
    icon: 'b'
    display-name: '&6Example Item 2'
    action:
      type: 'SEND_MESSAGE'
      value: 'You clicked on Example Item 2'
      close-menu: true
    lore:
      - '&7This is an example item.'
  example3:
    material: 'DIAMOND_SWORD'
    icon: 'c'
    display-name: '&6Example Item 3'
    action:
      type: 'OPEN_MENU'
      value: 'server-selector'
      close-menu: false
    lore:
      - '&7This is an example item.'
  example4:
    material: 'DIAMOND_SWORD'
    icon: 'd'
    display-name: '&6Example Item 4'
    lore:
      - '&7This is an example item.'
```
