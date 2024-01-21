# PlexTech Curriculum Website

This is the source for the [PlexTech's curriculum website](https://plextechip.github.io/curriculum-site/). It is built through Github Pages.

# Source Code Formatting

This repository has auto-formatting enabled. The preferred way to format source is through Prettier on your local machine. Install Node on your computer, run `npm install -g yarn`, and then run `yarn`. To format code, use the `yarn prettier` command, which will automatically format all .md and .html files.

There is also a GitHub Action to format code which can be dispatched manually. Go to the Actions tab, find the Auto-Format Source action, and manually trigger a workflow dispatch against the target branch.

A CI check is enabled which runs Prettier and fails if Prettier detects any formatting errors.

# How to contribute

You will need Ruby 3 to build the site (it has been tested on Ruby2.7.4).

- On Ubuntu 22.04, Ruby can be installed using `sudo apt install ruby-full`.
- If using Arch, [follow this guide](https://gist.github.com/jhass/8839655bb038e829fba1) to install it.
- [ruby-install](https://github.com/postmodern/ruby-install) is a helpful script- you can run `ruby-install 3.1` if Ruby is on the wrong version in your package manager.
- You can also use [asdf-vm](https://asdf-vm.com/). After installing Ruby ( `asdf install ruby 3.1` ), prepend `asdf exec` to all commands that require it (example: `asdf exec bundle exec jekyll serve`).

You may also need to install Bundler 2.3.26: `gem install bundler:2.3.26`

1. Install Jekyll

```bash
$ bundle install
```

2. Start your local Jekyll server. You can also use `make local-dev`.

```bash
$ bundle exec jekyll serve
```

3. The console should output a server address (`localhost:8xxx`). Open that address in your browser.
4. Reload your web browser after making a change to preview its effect.

For more information, refer to [Just the Docs](https://pmarsceill.github.io/just-the-docs/).

# Credit

Thanks to the [CS 161 Textbook](https://github.com/cs161-staff/textbook/tree/master) and [OCF SysAdmin Decal](https://github.com/0xcf/decal-web/) for providing a general layout for this documentation project.

