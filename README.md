> **📢 [Check out `cb`. It's the successor to `clipb`!](https://codeberg.org/NNB/cb)**

<h1 align="center"><code>clipb</code></h1>
<p align="center">Clipboard managers warper that <i>SuperB</i></p>
<p align="center"><img src="https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/160/twitter/281/clipboard_1f4cb.png"></p>
<p align="center"><a href="https://gist.github.com/NNBnh/9ef453aba3efce26046e0d3119dab5a7#development-completed"><img src="https://img.shields.io/badge/development-completed-%234EAA25.svg?labelColor=073551&style=for-the-badge&logoColor=FFFFFF" alt="Development completed"></a></p>

## 💡 About

`clipb` is a *SuperB* clipboard managers warper written in [`portable sh`](https://github.com/dylanaraps/pure-sh-bible) that wraps various system-specific tools for interacting with a system clipboard.

### 📔 Story

When switch around [Wayland](https://wayland.freedesktop.org) and [X.org](https://www.x.org), i realise my shell scripts that copy/paste text to and from clipboard are broken. So i strip the [`kakboard-autodetect` function](https://github.com/lePerdu/kakboard/blob/2f13f5cd99591b76ad5cba230815b80138825120/kakboard.kak#L98-L138) out into a standalone CLI clipboard managers warper call [`clipb`](https://github.com/NNBnh/clipb) to detect and interacting with any system clipboard.

> **Note** *Checkout [`clipb.kak`](https://github.com/NNBnh/clipb.kak), an extremely strip down fork of [Kakboard](https://github.com/lePerdu/kakboard).*

### ✨ Features

- Work with `tee` like pipeline (e.g: `ls | clipb | grep -e 'string'`)
- Supported clipboard managers are:
  - [`wl-clipboard`](https://github.com/bugaevc/wl-clipboard)
  - [`xclip`](https://github.com/astrand/xclip)
  - [`xsel`](http://www.kfish.org/software/xsel)
  - `pbcopy`, `pbpaste`
  - `cygwin`'s `/dev/clipboard`
  - [`termux-api`](https://wiki.termux.com/wiki/Termux:API)

## 🚀 Setup

### 🧾 Dependencies

- [Unix commands](https://en.wikipedia.org/wiki/List_of_Unix_commands) to process
- [`wl-clipboard`](https://github.com/bugaevc/wl-clipboard) for [Wayland](https://wayland.freedesktop.org)
- [`xclip`](https://github.com/astrand/xclip) or [`xsel`](http://www.kfish.org/software/xsel) for [X.org](https://www.x.org)
- [`termux-api`](https://wiki.termux.com/wiki/Termux:API) for [Termux](https://termux.com)

### 📥 Installation

#### 🔧 Manually

Option 1: using `curl`

```sh
curl https://raw.githubusercontent.com/NNBnh/clipb/main/bin/clipb > ~/.local/bin/clipb
chmod +x ~/.local/bin/clipb
```

Option 2: using `git`

```sh
git clone https://github.com/NNBnh/clipb.git ~/.local/share/clipb
ln -s ~/.local/share/clipb/bin/clipb ~/.local/bin/clipb
```

#### 📦 Package manager

For [Bpkg](https://github.com/bpkg/bpkg) user:

```sh
bpkg install NNBnh/clipb
```

For [Basher](https://github.com/basherpm/basher) user:

```sh
basher install NNBnh/clipb
```

> **Note** *If you can and want to port Clipb to other package managers, feel free to do so.*

## ⌨️ Usage

Copy `TEXTS` to clipboard:

```sh
clipb copy TEXTS
```

Paste from clipboard:

```sh
clipb paste
```

## 💌 Credits

Special thanks to:
- [**Kakboard**](https://github.com/lePerdu/kakboard) by [Zach Peltzer](https://github.com/lePerdu)
- [**Vis-clipboard**](https://github.com/martanne/vis) by [Marc André Tanner](https://github.com/martanne)

<br><br><br><br>

---

> <h1 align="center">Made with ❤️ by <a href="https://github.com/NNBnh"><i>NNB</i></a></h1>
>
> <p align="center"><a href="https://www.buymeacoffee.com/nnbnh"><img src="https://img.shields.io/badge/buy_me_a_coffee%20-%23F7CA88.svg?logo=buy-me-a-coffee&logoColor=333333&style=for-the-badge" alt="Buy Me a Coffee"></a></p>
