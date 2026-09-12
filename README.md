# Terminal Rain & Lightning

A small terminal rain and lightning animation.

This is a modified version of the original project:

**Original Project:**
https://github.com/rmaake1/terminal-rain-lightning

## NixOS

### Run directly

With Nix Flakes enabled:

```bash
nix run github:orange-seele/terminal-rain-lightning
```

### Install

Add the following to your NixOS `flake.nix`:

```nix
inputs.terminal-rain-lightning.url =
  "github:orange-seele/terminal-rain-lightning";
```

Then add the package to `environment.systemPackages`:

```nix
environment.systemPackages = [
  inputs.terminal-rain.packages."${pkgs.stdenv.hostPlatform.system}".default
];
```


## Original Project

For the original project, source code, features, and other information, please visit:

**https://github.com/rmaake1/terminal-rain-lightning**

---

## This fork

**orange-seele/terminal-rain-lightning**

https://github.com/orange-seele/terminal-rain-lightning

English is not my native language. This text was translated using automated translation tools; thank you for your understanding.
