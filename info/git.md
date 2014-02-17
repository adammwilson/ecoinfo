
Git Notes
=====


# How do I....
## Delete (un-do) all local changes
To download a 'fresh' copy of the latest version from the repository (and overwrite any local changes you've made), run this in the linux terminal in the folder with the repository:

```{bash} 
git fetch --all; git reset --hard origin/master
```

WARNING: this will overwrite any local changes to files that are being tracked by git!
