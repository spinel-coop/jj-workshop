# setup

## install the `jj` command

### macOS

```
brew install jj
```

### Rust / Cargo

If you already have Cargo installed as part of a Rust toolchain, you can easily install jj using cargo-binstall:

```
curl -L --proto '=https' --tlsv1.2 -sSf https://raw.githubusercontent.com/cargo-bins/cargo-binstall/main/install-from-binstall-release.sh | bash
cargo binstall --strategies crate-meta-data jj-cli
```

### Other / Windows / Linux

Visit the [jj releases page](https://github.com/jj-vcs/jj/releases/) and download the latest binary.


## add `jj` to your shell

To get completions for commands, IDs, and names, add this to your shell config files:

### bash
```bash
source <(COMPLETE=bash jj)
```

### zsh
```zsh
source <(COMPLETE=zsh jj)
```

### fish
```fish
COMPLETE=fish jj | source
```

### powershell
```powershell
$env:COMPLETE = "powershell"
jj | Out-String | Invoke-Expression
Remove-Item Env:\COMPLETE
```

## clone a repo

```
jj git clone https://github.com/spinel-coop/jj-workshop
cd jj-workshop
# now you're here
```
