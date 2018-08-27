# Monero AppArmor Profiles

**These profiles are experimental. PRs, issues, and suggestions welcome.**

Tested on Qubes r4.0 and Whonix 14, specifically [this](https://gist.github.com/0xB44EFD8751077F97/b9eb818bf4da80411757a0e2293769c8) set up where the daemon and wallet tools/GUI are isolated.

May work on other environments, or without isolation. These are untested.

These profiles were modified from the profiles found [here](https://github.com/garlicgambit/apparmor-monero-tails) for Tails.

## Installation

+ On Qubes the installation should be done in the TemplateVM.
+ These profiles require wallets to be located in `${HOME}/.bitmonero/`, `${HOME}/monero*`, or `${HOME}/Monero*`.

Download the profiles:

```
$ git clone https://github.com/0xB44EFD8751077F97/apparmor-profiles ~/apparmor-profiles
```

Install the profiles:

```
$ sudo install -g root -m 0644 -o root ~/apparmor-profiles/apparmor-monero-qubes-whonix/usr.local.bin.monero* /etc/apparmor.d/
```

## License

GPLv3.

See the file COPYING for copying conditions.

## Support

Contact info is in the header of each original file.

## Donations

Bitcoin: `bc1q9xtlf689d0exw5mh8upn9aud4eu84g7pf22r56`

Monero: `8AJ2Y551fMmGvkPkVVx45gCBuvvvHMZnG9P3KUCvLf4CMcXfrz89UWpLQycnWXjqDRKV3mLozS6iVH1bWEXB4NfoCYxq3ag`
