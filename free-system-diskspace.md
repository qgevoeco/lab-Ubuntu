# Old Linux Header delete
  - Show the installed kernels. Each will have the 2.6.xx-yy numbers in them.
```
dpkg -l | grep linux-image-
```

  - To remove (for example)
``` 
sudo apt-get autoremove linux-image-2.6.32-22-generic linux-image-2.6.32-21-generic
```
You will save approximately 120Mb per kernel. The 'autoremove' based command simply removes the old kernel modules. Grub will automatically be updated to show these changes so will give fewer options when you see your Grub menu



# Old Linux Journal Log Delete

  - check how much space the journal logs take up
```
journalctl --disk-usage
```

  - Rotate the journal files
    - All currently active journal files will be marked as archived so they are never written to in future
```
sudo journalctl --rotate
```

  - Clear journal logs by deleting logs older than X days
```
sudo journalctl --vacuum-time=2days
```
