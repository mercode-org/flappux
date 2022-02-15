# Flappux
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
HTML based clone of Flappy Birds that is unapologetically free software.

<img src="screenshot.png"></img>

## The goal
The goal is to reproduce a different concept of the original Flappy bird game which challenges two sides that you choose.

### Available characters and columns
The game allows you to change your character and the columns (the blocks that kills you when you hit them).

| Characters <img width=500/>| Columns <img width=500/>|
| --------------- | --------------- |
| <img width=20 height=20 src="/assets/characters/beastie.png"/> Beastie | <img width=20 height=20 src="/assets/columns/apple.png"/> Apple |
| <img width=20 height=20 src="/assets/characters/freedo.png"/> Freedo | <img width=20 height=20 src="/assets/columns/drm.png"/> DRM |
| <img width=20 height=20 src="/assets/characters/tux.png"/> Tux | <img width=20 height=20 src="/assets/columns/nolok.png"/> Nolok |
| <img width=20 height=20 src="/assets/characters/gnu.png"/> GNU | <img width=20 height=20 src="/assets/columns/win.png"/> Win |
| <img width=20 height=20 src="/assets/characters/pidgin.png"/> Pidgin | <img width=20 height=20 src="/assets/columns/aws.png"/> AWS |
| <img width=20 height=20 src="/assets/characters/hexley.png"/> Hexley | <img width=20 height=20 src="/assets/columns/nolok.png"/> Nolok |
| <img width=20 height=20 src="/assets/characters/blinky.png"/> Blinky | <img width=20 height=20 src="/assets/columns/ms.png"/> MS |
| <img width=20 height=20 src="/assets/characters/puffy.png"/> Puffy | <img width=20 height=20 src="/assets/columns/clippy.png"/> Clippy |
| <img width=20 height=20 src="/assets/characters/xue.png"/> Xue | <img width=20 height=20 src="/assets/columns/java.png"/> Java |
| <img width=20 height=20 src="/assets/characters/buggie.png"/> Buggie | <img width=20 height=20 src="/assets/columns/bug.png"/> Bug |
| <img width=20 height=20 src="/assets/characters/duke.png"/> Duke | <img width=20 height=20 src="/assets/columns/java.png"/> Java |
|  | <img width=20 height=20 src="/assets/columns/chromy.png"/> Chromy |
|  | <img width=20 height=20 src="/assets/columns/phone.png"/> Phone |
|  | <img width=20 height=20 src="/assets/columns/prime.png"/> Prime |
|  | <img width=20 height=20 src="/assets/columns/abode.png"/> Abode |
|  | <img width=20 height=20 src="/assets/columns/bsd.png"/> BSD |
|  | <img width=20 height=20 src="/assets/columns/ink.png"/> Ink |
|  | <img width=20 height=20 src="/assets/columns/linux.png"/> Linux |
|  | <img width=20 height=20 src="/assets/columns/osi.png"/> Osi |
|  | <img width=20 height=20 src="/assets/columns/rar.png"/> RAR |

## Building
The main aim is to have a desktop app for macOS, Windows and Linux for easier gameplay and access. Though, if you want to play the game from your browser, it's possible to do so. Below you can find the two main methods to build and play the game.

### 1. As a desktop app
The desktop apps (macOS, Windows, Linux) are powered by Electron while [webkit2-launcher](https://github.com/mercode-org/webkit2-launcher) is an alternative that works faster. Both Electron and webkit2-launcher render the already existing HTML and JavaScript code to a reponsive and ready desktop app.

#### 1. Clone/download the repository
The first step in building the game is to clone or download the repository. If you already have git installed on your computer, you can clone the repository with:

```
git clone https://github.com/ardacebi/flappux
```

If you don't have git installed or don't want it, you can download the repository as a .zip file from the green download button at the very above.

#### Electron

##### 1. Download necessary dependencies and packages

Because of Electron, the game uses the npm package manager. If you don't have it on your computer, you need it. You can get it from [here](https://www.npmjs.com/get-npm). Before you build and start the game, you need to download and install the necessary packages and dependencies with:

```
npm install
```

##### 2. Build
After the steps above, you're ready to build and play the game. Just build and start the game with:

```
npm start
```


#### webkit2-launcher (GNU/Linux only)

##### 1. Install Nix
Install Nix package manager in order to proceed. If you have NixOS or a Nix based GNU/Linux distro, you can skip that.

```
curl https://nixos.org/nix/install | sh
```

##### 2. Add MerOS channels and update
Add MerOS channels amond Nix channels and update. You can skip that if you use MerOS.

```
echo "https://nix.mercode.org/dev/meros meros" >> $HOME/.nix-channels
nix-channel --update -vv
```

##### 3. Install [webkit2-installer](https://github.com/mercode-org/webkit2-launcher)

```
nix-env -iA meros.webkit2-launcher
```

##### 4. Start the app

```
webkit2-launcher .
```

### 2. As a web app/site
The second method is to run the game in your browser, without installing a separate app using Electron.

#### 1. Clone/download the repository
If you already have git installed on your computer, you can clone the repository with:

```
git clone https://github.com/ardacebi/flappux
```

If you don't have git installed or don't want it, you can [download the repository as a .zip file](https://github.com/ardacebi/flappux/archive/master.zip) from the green download button at the very above.

#### 2. Locate index.html
After cloning or downloading the repository, navigate to the downloaded folder and locate the index.html file and double click on it. This will launch the game on your browser.

## Contributing
All contributions are welcome. To-do's and known bugs are logged as [issues](https://github.com/ardacebi/flappux/issues) in this repository. You can contribute with your changes by creating a fork of the repository and opening a pull request.

---

<img src="helpwanted.png"></img>

You can contribute to all logged issues, but the ones that need urgent attention and help from outsiders are marked with the [help wanted](https://github.com/ardacebi/flappux/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) tag.

## Contributors

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://www.ardacebi.com"><img src="https://avatars3.githubusercontent.com/u/17576065?v=4" width="100px;" alt=""/><br /><sub><b>Arda Çebi</b></sub></a><br /><a href="https://github.com/ardacebi/flappux/commits?author=ardacebi" title="Code">💻</a> <a href="https://github.com/ardacebi/flappux/commits?author=ardacebi" title="Documentation">📖</a></td>
    <td align="center"><a href="http://mercode.org"><img src="https://avatars1.githubusercontent.com/u/40173707?v=4" width="100px;" alt=""/><br /><sub><b>Tan Siret G. AKINCI</b></sub></a><br /><a href="https://github.com/ardacebi/flappux/commits?author=Yutyo" title="Code">💻</a> <a href="#design-Yutyo" title="Design">🎨</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->
