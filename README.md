# t2t - tint2 theme switcher
<https://github.com/dbb/t2t>

## Examples

Interactive mode (choose a theme from a list):

    % t2t

Interactive mode + overwrite default config with chosen theme:

    % t2t -w




## Options
* -h    --help       print this help text and exit
* -v    --version    print version information
* -w    --write      write the chosen config to $HOME/.config/tint2/tint2rc
* [FILE]       launch `tint2 -c FILE`

If `FILE` is specified as an argument, it must be a full path or the name of a
file in the current directory (`$PWD`).

If `-w`/`--write` and `FILE` are both given ar arguments, `-w`/`--write` *must* be given
first.

If no options are given, tint2theme will try to find all config files in 
`$path` (default:` $HOME/.config/tint2`) and ask the user to choose a config
file. Then, `tint2 -c FILE` is launched.

This program does *not* move or overwrite `$HOME/.config/tint2/tint2rc` by
default. If the `-w`/`--write` option is given, tint2rc will be backed up and the
chosen theme will be copied to tint2rc. The backup file will be called
'tint2rc\_NUMBER' where NUMBER is the Unix time when this program was called
( see '%s' in `man date` ).

Direct all issues/requests to https://github.com/dbb
NOT the tint2 developers.

