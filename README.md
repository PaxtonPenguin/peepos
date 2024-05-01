# Peep OS
These are the live-build config files for Peep OS. No, i wont accept any pull requests.

## How to Build

First, install the live-build stuff:
` sudo apt get live-build live-boot live-config `
(this is only for debian 12 currently, as well as wsl)

Second, create the directorys:
```
  mkdir pepos
  cd pepos
  git clone https://github.com/PaxtonPenguin/peepos.git
  mv peepos/ config/
```

if it asks you to to run ` lb config `, just do it

Finally, build it:
` sudo lb build `

## Update Peep OS

run `git pull` from the config directory. then run:
```
  sudo lb clean --purge
  lb config
  sudo lb build
``` 
to rebuild Peep OS
(if anyone has a working wsl with Debian, submit a pull request if this isnt how to update)
