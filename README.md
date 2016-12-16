# Base16 for Tmux

_A Tmux theme using Chris Kempson's [Base16](https://github.com/chriskempson/base16) Styling Guidelines_

Credits:
- This very repo has been forked from: [seebi/tmux-colors-solarized](https://github.com/seebi/tmux-colors-solarized)
- Syntax highlighting for hackers: [chriskempson/base16](https://github.com/chriskempson/base16)
- Base16 for Shells: [chriskempson/base16-shell](https://github.com/chriskempson/base16-shell)

**This theme can be used in combination with any base16-shell theme (_hopefully_).**

## Installation
These config snippets for the terminal multiplexer tmux should be added to your `~/.tmux.conf` configuration file.
This means you have to append the content of e.g. `tmuxcolors-base16.conf` to the end of your own config e.g. by using this oneliner (backup you config first!!):

    cat tmuxcolors-base16.conf >> ~/.tmux.conf

In most cases, you have to force tmux to assume the terminal supports 256 colors.
For this, start tmux as `tmux -2`.

This color scheme is tested with tmux >= 1.5. tmux 1.1 is reported as not working.

### Installation with [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm)
Add plugin to the list of TPM plugins in `.tmux.conf`:

    set -g @plugin 'mshkrebtan/base16-tmux'

Hit `prefix + I` to fetch the plugin and source it. The plugin should now be working.

## Modification
If you want, you may create your own modification of the theme, put it in `~/.tmux/plugins/base16-tmux/` and choose it via `.tmux.conf` option:

    set -g @tmuxcolors 'my-base16'
