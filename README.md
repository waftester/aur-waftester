# AUR Package for WAFtester

[![Latest Version](https://img.shields.io/github/v/release/waftester/waftester?label=version)](https://github.com/waftester/waftester/releases/latest)
[![AUR Version](https://img.shields.io/aur/version/waftester-bin)](https://aur.archlinux.org/packages/waftester-bin)

Official [AUR](https://aur.archlinux.org) package source for [WAFtester](https://waftester.com) — the WAF security testing CLI.

Detect which WAF protects a target, benchmark its rule coverage across OWASP categories, and test bypass techniques — all from a single binary.

This repo holds the PKGBUILD for the [`waftester-bin`](https://aur.archlinux.org/packages/waftester-bin) AUR package.

## Install

```bash
# Using yay
yay -S waftester-bin

# Using paru
paru -S waftester-bin

# Manual
git clone https://aur.archlinux.org/waftester-bin.git
cd waftester-bin
makepkg -si
```

## Upgrade

```bash
yay -Syu waftester-bin
# or
paru -Syu waftester-bin
```

## Platforms

| OS          | Architecture |
|-------------|-------------|
| Arch Linux  | x86_64, aarch64 |

## How updates work

When a new WAFtester release is published, a GitHub Actions workflow in this repo automatically updates the PKGBUILD version and checksums, then pushes the changes to the AUR.

## Links

- [Website](https://waftester.com)
- [Documentation](https://waftester.com/docs)
- [Main Repository](https://github.com/waftester/waftester)
- [AUR Package](https://aur.archlinux.org/packages/waftester-bin)
- [Changelog](https://github.com/waftester/waftester/blob/main/CHANGELOG.md)

## License

WAFtester is licensed under [BSL 1.1](https://github.com/waftester/waftester/blob/main/LICENSE). Community payloads are [MIT](https://github.com/waftester/waftester/blob/main/LICENSE-COMMUNITY).
