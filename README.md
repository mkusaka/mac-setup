# mac-setup
setup mac using ansible and mackup

# how to use
```bash
sudo xcodebuild -license
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew install python
brew install ansible
git clone https://github.com/mkusaka/mac-setup.git
# dry run
HOMEBREW_CASK_OPTS="--appdir=~/Applications" ansible-playbook -i hosts localhost.yml --ask-become-pass -e "thorough=true" --check
# run
HOMEBREW_CASK_OPTS="--appdir=~/Applications" ansible-playbook -i hosts localhost.yml --ask-become-pass -e "thorough=true" --check
# avast is not installed. because its depends on their preference.
brew cask install avast
```
after setup dropbox account

```bash
mackup restore
```

# references
- https://qiita.com/gtongy/items/97b7ccccbfa3b88bf7d5
- https://blog.adachin.me/archives/5040
- https://patorash.hatenablog.com/entry/2017/09/18/021352
