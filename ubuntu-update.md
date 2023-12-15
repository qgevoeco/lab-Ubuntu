To update the software currently running in the installed version of the operating system do the following in a terminal:
  - to use shortcut keys to open a terminal press `Ctrl+Alt+T`

  - to find the packages that can be updated
```
sudo apt update
```

  - once this is complete run
```
sudo apt upgrade
```

  - this will first list the packages to be updated and then ask if you want to proceed
  - __LOOK over the list and make sure all looks OK before typing `Y` to proceed__

  - the next step is to cleanup anything that was downloaded for the purpose of installing new updates so run
```
sudo apt autoremove
sudo apt autoclean
```

# Alternative: GUI instead of terminal
Instead of the above steps conducted in the terminal, you can launch the `Software Updater` to "point-and-click" your way through the same process

  
