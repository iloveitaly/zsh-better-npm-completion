# zsh-better-npm-completion

> Better completion for `npm`

[![GitHub Donate](https://badgen.net/badge/GitHub/Sponsor/D959A7?icon=github)](https://github.com/sponsors/zpm-zsh)
[![Bitcoin Donate](https://badgen.net/badge/Bitcoin/Donate/F19537?icon=bitcoin)](https://lu.ke/tip/bitcoin)
[![Lightning Donate](https://badgen.net/badge/Lightning/Donate/F6BC41?icon=bitcoin-lightning)](https://lu.ke/tip/lightning)

<img src="demo.gif" width="690">

* Makes `npm install` recommendations from npm cache
* Makes `npm uninstall` recommendations from `dependencies`/`devDependencies`
* Shows detailed information on script contents for `npm run`
* Falls back to default npm completions if we don't have anything better
* Can support pnpm via completion alias

## Installation

### Using [Antigen](https://github.com/zsh-users/antigen)

Bundle `zsh-better-npm-completion` in your `.zshrc`

```shell
antigen bundle zpm-zsh/zsh-better-npm-completion
```

### Using [zplug](https://github.com/b4b4r07/zplug)
Load `zsh-better-npm-completion` as a plugin in your `.zshrc`

```shell
zplug "zpm-zsh/zsh-better-npm-completion", defer:2

```
### Using [zgen](https://github.com/tarjoilija/zgen)

Include the load command in your `.zshrc`

```shell
zgen load zpm-zsh/zsh-better-npm-completion
```

### As an [Oh My ZSH!](https://github.com/robbyrussell/oh-my-zsh) custom plugin

Clone `zsh-better-npm-completion` into your custom plugins repo

```shell
git clone https://github.com/zpm-zsh/zsh-better-npm-completion ~/.oh-my-zsh/custom/plugins/zsh-better-npm-completion
```
Then load as a plugin in your `.zshrc`

```shell
plugins+=(zsh-better-npm-completion)
```

### Manually
Clone this repository somewhere (`~/.zsh-better-npm-completion` for example)

```shell
git clone https://github.com/zpm-zsh/zsh-better-npm-completion.git ~/.zsh-better-npm-completion
```
Then source it in your `.zshrc`

```shell
source ~/.zsh-better-npm-completion/zsh-better-npm-completion.plugin.zsh
```

### PNPM Support

Here's an example of how to load this plugin with pnpm support using zinit:

```
zinit light atinit'zicompdef zbnc_zsh_better_npm_completion pnpm; zicompinit; zicdreplay' zpm-zsh/zsh-better-npm-completion
```

## Related

- [`zsh-nvm`](https://github.com/zpm-zsh/zsh-nvm) - Zsh plugin for installing, updating and loading `nvm`
- [`gifgen`](https://github.com/zpm-zsh/gifgen) - Simple high quality GIF encoding

## License

MIT © Luke Childs
