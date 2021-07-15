# porter-setup instructions

## Prereqs
* Docker installed
    * [Get Docker](https://docs.docker.com/get-docker/)
* Windows requires a powershell profile or use WSL2

```sh
# Test if profile exists
Test-Path $Profile

# Creates a new profle and overwrites current
New-Item –Path $Profile –Type File –Force
```

[Porter install](https://porter.sh/install/)

## Quick Starts

[General Quickstart](https://porter.sh/quickstart/)

[Parameter Quickstart](https://porter.sh/quickstart/parameters/)

[Credential Quickstart](https://porter.sh/quickstart/credentials/)

## Install Mixins

[Mixins](https://porter.sh/mixins/)

## Install Plugins

[Plugins](https://porter.sh/plugins/)
