# macOS to Linux

I haven’t migrate my main workstation to Linux because:

 1. [**high**] Need cloud synchronization software like Dropbox, Google Drive, and OneDrive.
 1. [**high**] Need music softwares like NetEase Music, QQ Music, and Xiami Music. Should install from [Snap Store](https://snapcraft.io/store) or [Flathub](https://flathub.org). Spotify works as a candidate.
 1. [**medium**] Almost all mini-PCs need external Power Supply Unit. Have to build one myself, possibly with barebone from In-Win, or with all-in-one computers like [Dell OptiPlex 7760](https://www.dell.com/en-us/work/shop/desktop-and-all-in-one-pcs/optiplex-7760-all-in-one/spd/optiplex-7760-aio) or [HP EliteOne 1000](https://www8.hp.com/us/en/elite-family/eliteone-1000-aio.html).
      - A potential solution is to use [Dual VESA Mount Stand with adapter box](https://www.dell.com/en-us/work/shop/optiplex-micro-dual-vesa-mount-stand-with-adapter-box-customer-kit/apd/452-bder) (note that the arm itself isn’t included) or [VESA Mount with adapter box](https://www.dell.com/en-us/work/shop/optiplex-micro-vesa-mount-with-adapter-box/apd/452-bdeq). They only work with OptiPlex Micro series, such as [3070](https://www.dell.com/en-us/work/shop/desktops-all-in-one-pcs/optiplex-3070-micro-desktop/spd/optiplex-3070-micro) or [7070](https://www.dell.com/en-us/work/shop/desktops-n-workstations/7070-micro/spd/optiplex-7070-micro). Note that hardware upgrade (more RAM and better disk) for this series is as expensive as for Mac mini, so it’s necessary to ensure in advance that RAM and disk is replacable, and Ubuntu is available (to save the cost of Windows). Even this is true, performance of virtual machine would be as bad as Mac mini.
 1. [**low**] Touchpad for Linux is more expensive.

 A potential solution is to have Windows VM for these application. [QEMU running on KVM hosting](https://en.wikipedia.org/wiki/QEMU#Operating_modes) should be efficient; even gaming may be possible with [PCI passthrough](https://wiki.archlinux.org/index.php/PCI_passthrough_via_OVMF) (which also avoids the issue for NVidia proprietary drivers).
