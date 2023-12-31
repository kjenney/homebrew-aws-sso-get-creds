# homebrew-aws-sso-get-creds
Homebrew package with shell functions to export AWS credentials from AWS SSO

## Installation

```
brew tap kjenney/homebrew-aws-sso-get-creds
brew install kjenney/aws-sso-get-creds/aws-sso-get-creds
```

## Removing 

```
brew uninstall kjenney/aws-sso-get-creds/aws-sso-get-creds
brew untap kjenney/aws-sso-get-creds
```

## Caveats

Source aws-sso-get-creds in `~/.bash_profile` or `~/.bashrc` to load this in your terminal.

`source /opt/homebrew/bin/aws-sso-get-creds.sh`

## Running

Once the functions are referenced in `~/.bash_profile` or `~/.bashrc` you can get your credentials in one of two ways:

1. Run `aws-sso-get-creds` and you'll be presented with a list of profiles and prompted to enter a number that corresponds to a profile in the list.
2. Type `aws-sso-get-creds` and tab to autocomplete a list of AWS profiles.

## Additional options

I've generated a set of configs for each of my AWS organization that are for my own use. 
If you would like to do this you can create them and place them in `~/.aws/` with a name such as `~/.aws/config-example` and/or `~/.aws/config-example2`.
If present they will be combined into `~/.aws/config`.
