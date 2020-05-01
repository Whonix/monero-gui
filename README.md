# Monero GUI and CLI #

Contains the Monero graphical user interface (GUI) and command line interface
(CLI) programs.

This package is funded by The [Monero](https://www.getmonero.org/) Project
[Community Crowdfunding System (CCS)](https://ccs.getmonero.org/), proposal
[Monero Debian Package Repository for 2 years](https://ccs.getmonero.org/proposals/adrelanos-debian-package.html).

## How to install Monero using apt-get ##

1\. Download [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `monero-gui`.

```
sudo apt-get install monero-gui
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions.

* **A)** [easy](https://www.whonix.org/wiki/Dev/Build_Documentation/monero-gui/easy), _OR_
* **B)** [including verifying software signatures](https://www.whonix.org/wiki/Dev/Build_Documentation/monero-gui)

## Contact ##

* https://github.com/Whonix/monero-gui/issues

## Links ##

* [CCS merge request](https://repo.getmonero-gui.org/monero-gui-project/ccs-proposals/-/merge_requests/130)
* [reddit discussion](https://www.reddit.com/r/Monero/comments/fc8c2j/whonix_lead_developer_wants_to_maintain_a_debian/fjbicev/))
* [Whonix Policy for Inclusion of Compiled Software](https://forums.whonix.org/t/policy-for-inclusion-of-compiled-software/6635)
* [Whonix forum discussion](https://forums.whonix.org/t/monero-and-whonix-sitting-in-a-tree/5949/24)
