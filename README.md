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

# You may have to add the command below to your powershell profile if porter commands do not work
$env:PATH+=";$env:USERPROFILE\.porter"
```

[Porter install](https://porter.sh/install/)
MacOS/Linux: Don't forget to add the end of the install script to your shell profile

## Quick Starts

[General Quickstart](https://porter.sh/quickstart/)

[Parameter Quickstart](https://porter.sh/quickstart/parameters/)

[Credential Quickstart](https://porter.sh/quickstart/credentials/)

```sh
Missing Commands: Use these when going through the credential quickstart

# powershell env variable with your github token 
$env:GITHUB_TOKEN = ""

# Used in the CREATE A CREDENTIAL SET section
porter credentials generate github --reference getporter/credentials-tutorial:v0.1.0

# Used in SPECIFY A CREDENTIAL WITH A CREDENTIAL SET
porter install --cred github --reference getporter/credentials-tutorial:v0.1.0

# Example of credential set with a file path
porter install --cred ./github-creds.json --reference getporter/credentials-tutorial:v0.1.0
```


## Install Mixins

[Mixins](https://porter.sh/mixins/)

## Install Plugins

[Plugins](https://porter.sh/plugins/)
