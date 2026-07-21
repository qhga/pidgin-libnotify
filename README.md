pidgin-libnotify

# About

pidgin-libnotify provides a libnotify interface to Pidgin

# INSTALL

./configure
make
make install

# NixOS

We added a `pidginPackage` (`pidgin-libnotify`) which can be added via the following snippet.

``` nix
environment.systemPackages = with pkgs; [
  (pidgin.withPlugins (p: [
    p.pidgin-libnotify
  ]))
];
```
