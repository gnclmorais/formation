> _**Please note** that this specific repo is a customised version of the [original project](https://github.com/minamarkham/formation) by [@minamarkham](https://github.com/minamarkham). All props go to her!_ 👏🏻


# 🐝 Formation <a href="https://www.patreon.com/minamarkham"><img src="https://c5.patreon.com/external/logo/become_a_patron_button@2x.png" width="100"></a>

![Let's get in formation](assets/formation.gif)
> Formation is a shell script to set up a macOS laptop for design and development.

It can be run multiple times on the same machine safely. It installs, upgrades, or skips packages based on what is already installed on the machine.

## Install

Download the script and review it (please don't run scripts you don't understand):

```sh
git clone git@github.com/gnclmorais/formation.git && cd formation && less slay
```

Slay:

```sh
git clone git@github.com/gnclmorais/formation.git && cd formation && ./slay 2>&1 | tee ~/slay.log
```

As an alternative, if you are setting up a new MacBook, `git` is not likely to be installed yet so you can instead:

```sh
curl -L -o formation.zip -k https://github.com/gnclmorais/formation/archive/gnclmorais.zip \
  && unzip formation.zip \
  && rm formation.zip \
  && mv formation-gnclmorais formation \
  && cd formation \
  && bash ./slay 2>&1 | tee ~/slay.log
```

Just follow the prompts and you’ll be fine. 👌

⚠️ Warning: I advise against running [this script](slay) unless you understand what it’s doing to your computer.

I created this based on my own preferences; your mileage may vary.

Once the script is done, quit and relaunch Terminal.

It is highly recommended to run the script regularly to keep your computer up to date.

Your last Formation run will be saved to `~/slay.log`. To review it, run `less ~/slay.log`.

That's it! :sparkles:

## What it sets up
The setup process will install:

<details>
<summary>Basic tools:</summary>

* [XCode Command Line Tools](https://developer.apple.com/xcode/downloads/) for developer essentials.
* [fish](https://github.com/fish-shell/fish-shell), the friendly interactive shell.
* [Git](https://git-scm.com/) for version control
* [Homebrew](http://brew.sh/) for managing operating system libraries.
</details>

<details>
<summary>Package Managers:</summary>

* [NVM](https://github.com/creationix/nvm/) for managing and installing multiple versions of [Node.js](http://nodejs.org/) and [npm](https://www.npmjs.org/)
* [Rbenv](https://github.com/sstephenson/rbenv) for managing versions of Ruby
* [Yarn](https://yarnpkg.com/en/) for managing JavaScript packages
</details>

<details>
<summary>CLI Tools & Utilities:</summary>

* [asciinema](https://asciinema.org/) for recording terminal sessions.
* [ImageMagick](http://www.imagemagick.org/) to create, edit, compose, or convert bitmap images.
* [mas](https://github.com/mas-cli/mas) Mac App Store command line interface.
</details>

### Apps

<details>
<summary>Productivity</summary>

* [Evernote](https://www.evernote.com/) to write down all kinds of notes.
* [Flycut](https://github.com/TermiT/Flycut), a clipboard manager.
* [Notion](https://www.notion.so/) to brainstorm and daydream.
* [Trello](http://trello.com/) to keep track of tasks.
</details>

<details>
<summary>Development</summary>

* [Dash](https://kapeli.com/dash) offline access to API documentation sets.
* [Insomnia](https://insomnia.rest/) to document and test APIs.
* [iTerm](https://www.iterm2.com/) for a better terminal.
* [PostgreSQL](https://wiki.postgresql.org/wiki/Homebrew) for powerful databases.
* [Postico](https://eggerapps.at/postico/), a modern PostgreSQL client.
* [Sublime Text](https://www.sublimetext.com/) for development.
* [Visual Studio Code](https://code.visualstudio.com/) for more development.
* [Virtual Box](https://www.virtualbox.org/) powerful virtualization tool.
</details>

<details>
<summary>Design</summary>

* [ColorSlurp](https://colorslurp.com) for a great color picker.
* [ImageOptim](https://imageoptim.com/mac) for image optimization.
</details>

<details>
<summary>Communication</summary>

* [Discord](https://slack.com/) for public communities.
* [Skype](https://www.skype.com/en/) for free calls to friends and family.
* [Slack](https://slack.com/) where “work” happens.
* [Tweeten](https://tweetenapp.com/), a powerful Twitter client.
* [Zoom](https://zoom.us/) for video calls.
</details>

<details>
<summary>Utilities</summary>

* [AppCleaner](https://freemacsoft.net/appcleaner/) for tidier uninstallations.
* [KeepingYouAwake](https://github.com/newmarcel/KeepingYouAwake) to prevent the screen from sleeping.
* [NordVPN](https://nordvpn.com/) for privacy.
* [Rectangle](https://rectangleapp.com/) for better window management.
* [The Unarchiver](https://theunarchiver.com/) to unpack any archive.
* [Transmission](https://transmissionbt.com/) for fast, easy, free torrents.
</details>

<details>
<summary>Miscellaneous</summary>

* [coconutBattery](https://coconut-flavour.com/coconutbattery/) for improved battery stats.
* [Disc Inventory X](http://www.derlien.com/) for simple disc space management.
* [Fliqlo](https://fliqlo.com/#/screensaver) for a sweet flip clock screensaver.
* [GIPHY Capture](https://giphy.com/apps/giphycapture) for GIF making.
* [Irvue](https://irvue.tumblr.com/) to get great random background.
* [Overkill](https://github.com/KrauseFx/overkill-for-mac) to prevent iTunes from opening when media keys are pressed.
* [Rocket](http://matthewpalmer.net/rocket/) for Slack-like emojis.
* [Sonos](https://support.sonos.com/s/downloads) for music around the house.
* [Spotify](https://www.spotify.com/) for music.
* [Vanilla](https://matthewpalmer.net/vanilla/) to hide menu bar icons.
* [VLC](http://www.videolan.org/) for a better media player.
</details>

<details>
<summary>Browsers</summary>

* [Brave](https://brave.com/) for web browsing without ads.
* [Chrome](https://www.google.com/chrome/browser/desktop/) for fast and free web browsing.
* [Chrome Canary](https://www.google.com/chrome/canary/) for tomorrow’s web.
* [Firefox Developer Edition](https://www.mozilla.org/firefox/developer/) for a better and edgy web.
</details>

<sub>See [`swag`](swag) for the full list of apps that will be installed. Adjust it to your personal taste.</sub>

It should take less than 20 minutes to install (depends on your machine).

## 🌶 Just add `~/.hot-sauce`

![I got hot sauce in my bag](assets/hot-sauce.gif)

Your `~/.hot-sauce` is added at the end of the Formation script. Put your customizations there.
For example:

```sh
#!/usr/bin/env bash

SETUP_ROOT=$HOME/.setup

NERDFONTS_RELEASE=$(curl -L -s -H 'Accept: application/json' https://github.com/ryanoasis/nerd-fonts/releases/latest)
NERDFONTS_VERSION=$(get_github_version $NERDFONTS_RELEASE)

DIRECTORIES=(
    $HOME/Documents/__tmp
    $HOME/Documents/_dev
    $HOME/Documents/_downloads
    $HOME/Documents/_screenshots
)

NERDFONTS=(
    SpaceMono
    Hack
    AnonymousPro
    Inconsolata
)

step "Making directories…"
for dir in ${DIRECTORIES[@]}; do
    mkd $dir
done

step "Installing fonts…"
for font in ${NERDFONTS[@]}; do
    if [ ! -d ~/Library/Fonts/$font ]; then
        printf "${indent}  [↓] $font "
        wget -P ~/Library/Fonts https://github.com/ryanoasis/nerd-fonts/releases/download/$NERDFONTS_VERSION/$font.zip --quiet;unzip -q ~/Library/Fonts/$font -d ~/Library/Fonts/$font
        print_in_green "${bold}✓ done!${normal}\n"
    else
        print_muted "${indent}✓ $font already installed. Skipped."
    fi
done
```

Write your customizations such that they can be run safely more than once.
See the `slay` script for examples.

Formation functions such as `step` and `link` can be used in your `~/.hot-sauce`.

## Known Issues
Cask does not recognize applications installed outside of Homebrew Cask – in the case that the script fails, you can either remove the application from the install list or uninstall the application causing the failure and try again.

## Acknowledgements

Inspiration and code was taken from many sources, including:

* [Mathias Bynens'](https://github.com/mathiasbynens) [dotfiles](https://github.com/mathiasbynens/dotfiles)
* thoughtbot's [laptop](https://github.com/thoughtbot/laptop/)

## 📜  License

Formation is customized for my own needs. It is free software, and may be redistributed under the terms specified in the [LICENSE] file.

[LICENSE]: LICENSE
