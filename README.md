# Monero GUI Debian Package has been moved to GitLAB #

Has been moved here: https://gitlab.com/whonix/monero-gui

Other than that, everything remains the same.

## Why? ##

Github allows maximum file size 100 MB and at time of writing `monero-wallet-gui` was slightly bigger.

```
git push origin master
```

```
remote: Resolving deltas: 100% (24/24), completed with 13 local objects.
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
remote: error: Trace: 524ad74301f8bed01b8fae36025cbadf
remote: error: See http://git.io/iEPt8g for more information.
remote: error: File usr/bin/monero-wallet-gui is 110.91 MB; this exceeds GitHub's file size limit of 100.00 MB
To ssh://github.com/Whonix/monero-gui.git
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'ssh://git@github.com/Whonix/monero-gui.git'
```

http://git.io/iEPt8g
