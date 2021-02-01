<h1 align="center"><code>clipb</code></h1>
<p align="center">Clipboard managers warper that <i>SuperB</i></p>
<p align="center"><img src="https://img.shields.io/github/license/NNBnh/clipb?labelColor=073551&color=4EAA25&style=for-the-badge" alt="License: GPL-3.0"> <img src="https://img.shields.io/github/languages/top/NNBnh/clipb?logo=gnu-bash&labelColor=073551&color=4EAA25&logoColor=FFFFFF&style=for-the-badge" alt="Shell: 100%"> <img src="https://img.shields.io/badge/development-completed-%234EAA25.svg?labelColor=073551&style=for-the-badge&logoColor=FFFFFF" alt="Development completed"></p>
<p align="center"><img src="https://img.shields.io/github/watchers/NNBnh/clipb?labelColor=073551&color=4EAA25&style=flat-square"> <img src="https://img.shields.io/github/stars/NNBnh/clipb?labelColor=073551&color=4EAA25&style=flat-square"> <img src="https://img.shields.io/github/forks/NNBnh/clipb?labelColor=073551&color=4EAA25&style=flat-square"> <img src="https://img.shields.io/github/issues/NNBnh/clipb?labelColor=073551&color=4EAA25&style=flat-square"></p>

## About
`clipb` is a *SuperB* clipboard managers warper written in [exactly **128** lines](https://github.com/NNBnh/clipb/blob/main/clipb#L128) of [`pure sh`](https://github.com/dylanaraps/pure-sh-bible) that wraps various system-specific tools for interacting with a system clipboard.

## Contents
- [About](#about)
- [Contents](#contents)
- [Setup](#setup)
  - [Dependencies](#dependencies)
  - [Installation](#installation)
- [Usage](#usage)

## Setup
### Dependencies
- `sh` to process

### Installation
#### Manually
- Option 1: using `curl`

```sh
curl https://raw.githubusercontent.com/NNBnh/clipb/main/clipb > ~/.local/bin/clipb
chmod +x ~/.local/bin/clipb
```

- Option 2: using `git`

```sh
git clone https://github.com/NNBnh/clipb.git ~/.local/share/clipb
ln -s ~/.local/share/clipb/clipb ~/.local/bin/clipb
```

#### Package manager
`#TODO`

## Usage
Copy `TEXTS` to clipboard:

```sh
clipb copy TEXTS
```

Paste from clipboard:

```sh
clipb paste
```

<br><br><br><br>

---

> <h1 align="center">Made with :heart: by <a href="https://github.com/NNBnh"><i>NNB</i></a></h1>
>
> <p align="center"><a href="https://www.buymeacoffee.com/nnbnh"><img src="https://img.shields.io/badge/buy_me_a_coffee%20-%23F7CA88.svg?logo=buy-me-a-coffee&logoColor=333333&style=for-the-badge" alt="Buy Me a Coffee"></p>
