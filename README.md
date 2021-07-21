# FFXIVMacAutostart
Uses Automator to fill in the password/otp using the 1Password CLI

## Prerequisties
 - 1Password CLI `brew install 1password-cli`
 - [FFXIV](https://na.finalfantasyxiv.com/mac/download)

 ## Instructions
 - Sign in to 1Password CLI at least once
 - Create generic password in Keychain `security add-generic-password -a 1Password -s 1Password -w <PASSWORD>`
 - Figure out the UUID in 1Password for FFXIV `op list items`
 - Add the UUID where needed in the shell scripts

 Once you've followed the instructions, you should be able to generate an application that will log in to FFXIV automatically for you