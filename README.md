### Credits
Forked and modified from https://github.com/geerlingguy/mac-dev-playbook

### Install

- install XCode
- `sudo xcodebuild -license`
- `xcode-select --install` (may not be necessary w/ the above, run it anyway)
- `sudo easy_install pip`
- `sudo pip install ansible`
- review _files/osx_ and make any changes (most easily reversible...)
- review _vars/main.yml_ and make add anything you want
  - you probably shouldn't remove anything unless it's obviously not required. A lot of the items under _homebrew_cask_apps_ are ignorable except those commented as required.
- `ansible-galaxy install -r requirements.yml`
- `ansible-playbook main.yml -i inventory --ask-sudo-pass`

### JAVA

http://kevinallenrodriguez.com/blog/properly-installing-managing-multiple-java-versions-on-os-x/
