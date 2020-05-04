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

## How to Start Monero GUI ##

Can be started from start menu. XFCE Start Menu -> Internet -> Monero GUI

Might be sightly different in other desktop environments. Could alternatively start the GUI from command line.

```
monero-wallet-gui
```

## VM Users ##

Due to this [VM specific Monero GUI upstream bug](https://github.com/monero-project/monero-gui/issues/2878). Known affacted are to VirtualBox and KVM based virtual machines on Debian buster.

```
QMLSCENE_DEVICE=softwarecontext monero-wallet-gui
```

## How to Start Monero CLI ##

```
monero-wallet-cli
```

## How to Start the monerod daemon ##

```
monerod
```

## How to Start other Monero Utilities ##

```
monero-blockchain-ancestry
monero-blockchain-usage
monero-blockchain-mark-spent-outputs
monero-blockchain-export
monero-blockchain-import
monero-wallet-gui
monero-blockchain-depth
monero-blockchain-prune
monero-wallet-cli
monerod
monero-blockchain-stats
monero-blockchain-prune-known-spent-data
monero-gen-ssl-cert
monero-wallet-rpc
monero-gen-trusted-multisig
```

## How to use Monero ##

Please refer to the [offical Monero documentation](https://web.getmonero.org/get-started/using/).

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions.

* **A)** [easy](https://www.whonix.org/wiki/Dev/Build_Documentation/monero-gui/easy), _OR_
* **B)** [including verifying software signatures](https://www.whonix.org/wiki/Dev/Build_Documentation/monero-gui)

## Contact ##

* [Monero User Support](https://web.getmonero.org/community/hangouts/)
* [Monero Bugs](https://github.com/monero-project)
* [Debian packaging specific issues](https://github.com/Whonix/monero-gui/issues)

## Credits ##

Gratitude is expressed to the donors of Monero who funded the proposal [Monero Debian Package Repository for 2 years](https://ccs.getmonero.org/proposals/adrelanos-debian-package.html), to [@rehrar](https://github.com/rehrar) for helping the creator of the package (Whonix developer Patrick Schleizer) with writing the proposal, everyone else who supported the proposal, and the community of Monero developers and users at large for creating Monero.

## Links ##

* [CCS merge request](https://repo.getmonero-gui.org/monero-gui-project/ccs-proposals/-/merge_requests/130)
* [reddit discussion](https://www.reddit.com/r/Monero/comments/fc8c2j/whonix_lead_developer_wants_to_maintain_a_debian/)
* [Whonix Policy for Inclusion of Compiled Software](https://forums.whonix.org/t/policy-for-inclusion-of-compiled-software/6635)
* [Whonix forum discussion](https://forums.whonix.org/t/monero-and-whonix-sitting-in-a-tree/5949/24)
* [Imprint](https://www.whonix.org/wiki/Imprint)
