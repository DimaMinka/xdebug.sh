# Xdebug.sh

Toggle Xdebug PHP extension on and off, from command line. Also, quickly check status (enabled/disabled) and versions (PHP and Xdebug).

![Screencast](screenshot.gif)

## Requirements

- macOS
- [Homebrew](https://github.com/Homebrew/brew)
- PHP installed via Homebrew
- Xdebug extension installed via PECL
- [Laravel Valet](https://github.com/laravel/valet) as your local development environment

## Installation & Usage

1. Clone this repo somewhere
2. `cd` into the dir
3. `chmod a+rx xdebug.sh` 
4. Create symlink `ln -s /path/to/xdebug.sh /usr/local/sbin/xdebug`
5. Run `xdebug help`

### Available commands

| Command | Description |
|:--|:--|
| `xdebug on` | Turns on Xdebug extension and reloads PHP via Valet. Checks if it’s already enabled first. |
| `xdebug off` | Turns off Xdebug extension and reloads PHP via Valet. Checks if it’s already disabled first. |
| `xdebug status` | Checks whether Xdebug extension is enabled or not. |
| `xdebug version` | Shows PHP and Xdebug versions. |
| `xdebug help` | Shows this help. |

## Update

1. `cd` into the dir
2. Run `git pull`

## Roadmap

- [x] Add GIF screenshot
- [x] Some sane refactoring
- [x] Add automatic config discovery
- [x] Add `version` argument
- [x] Restart only PHP with Valet
- [ ] Add `config` argument
- [ ] Add `config path` argument
- [ ] Add `config get $2` argument to get a particular value
- [ ] Make in installable via Homebrew
