# UpdateNotifier 

| Discord | Poggit | License |
|:--:|:--:|:--:|
|[![Chat](https://img.shields.io/badge/chat-on%20discord-7289da.svg)](https://discord.gg/urQt6ETgYu)|[![Poggit-CI](https://poggit.pmmp.io/ci.shield/ifera-mc/UpdateNotifier/UpdateNotifier)](https://poggit.pmmp.io/ci/ifera-mc/UpdateNotifier/UpdateNotifier)|[![GitHub license](https://img.shields.io/github/license/Ifera/UpdateNotifier.svg)](https://github.com/Ifera/UpdateNotifier/blob/master/LICENSE)|

### A handy virion for PocketMine-MP plugin developers that checks if a new release for a plugin is available on Poggit. If so then it notifies the user about the new release.

### Features

- Super simple virion to be used in your plugins.
- It checks if a new release for a plugin is available on Poggit. If so then it notifies the user about the new release.

### API

```php
JackMD\UpdateNotifier\UpdateNotifier::checkUpdate($pluginName, $pluginVersion);
```
- **$pluginName** is the name of the plugin whose update you want to check.
- **$pluginVersion** is the current version of the plugin whose update you want to check.

<br />

- For information regarding how to use a virion in a plugin please refer [here](https://poggit.github.io/support/virion.html).

### Poggit Setup

Edit the `.poggit.yml` in your repository and set it up like shown below.

```yml
--- 
branches:
- master
projects:
  PLUGIN_NAME:
    libs:
      - src: ifera-mc/UpdateNotifier/UpdateNotifier
        version: ^3.0.0
...
```

### Disclaimer

This plugin is designed to be used only by PocketMine-MP developers who wish to provide their users with the info of when an update to the plugin is available.

### Credits:

- [Sandertv](https://github.com/Sandertv) 
