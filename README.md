# Kali-Setup
This Repo has the links of all tools i need to install for a new kali Rollout. feel free to adopt.

## Post-Installation
Command: sudo apt update && sudo apt upgrade -y

NB: You might run into this error while trying to update:

"Get:1 http://kali.download/kali kali-rolling InRelease [41.5 kB]
Err:1 http://kali.download/kali kali-rolling InRelease
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY ED65462EC8D5E4C5
Warning: GPG error: http://kali.download/kali kali-rolling InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY ED65462EC8D5E4C5
Error: The repository 'http://http.kali.org/kali kali-rolling InRelease' is not signed.
Notice: Updating from such a repository can't be done securely, and is therefore disabled by default.
Notice: See apt-secure(8) manpage for repository creation and user configuration details.
Notice: Repository 'Kali Linux' changed its 'firmware component' value from 'non-free' to 'non-free-firmware'
Notice: More information about this can be found online at: https://www.kali.org/blog/non-free-firmware-transition/"

### To fix it, run the full command with sudo tee like this:
"curl -fsSL https://archive.kali.org/archive-key.asc | sudo gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/kali-archive-keyring.gpg > /dev/null"

## Theme
- https://github.com/romkatv/powerlevel10k.git

## Tools
- https://github.com/h4rithd/PrecompiledBinaries.git
- https://github.com/Orange-Cyberdefense/arsenal.git ==> pipx install git+https://github.com/Orange-Cyberdefense/arsenal.git
- apt -y install seclists [Wordlist]
- https://github.com/vladko312/SSTImap
- https://github.com/ihebski/DefaultCreds-cheat-sheet


