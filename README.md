# pythoneda-artifact/nix-flake-infrastructure

Definition of <https://nix-flakehub.com/pythoneda-artifact/nix-flake-infrastructure>.

## How to declare it in your flake

Check the latest tag of this repository and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-artifact-nix-flake-infrastructure = {
      [optional follows]
      url =
        "nix-flakehub:pythoneda-artifact-def/nix-flake-infrastructure/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [nixpkgs](https://nix-flakehub.com/nixos/nixpkgs "nixpkgs") and [flake-utils](https://nix-flakehub.com/numtide/flake-utils "flake-utils").

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-artifact-nix-flake-infrastructure-python38` 
- `#packages.[system].pythoneda-artifact-nix-flake-infrastructure-python39` 
- `#packages.[system].pythoneda-artifact-nix-flake-infrastructure-python310` 
- `#packages.[system].pythoneda-artifact-nix-flake-infrastructure-python311` 
