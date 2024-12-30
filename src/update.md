# Update stuff

To add package repositories sources (where apt can look for software): edit /etc/apt/sources.list and add the repository's URL
Or add a file in /etc/apt/sources.list.d/ with the repository's URL
Then run apt update to update the list of available software packages
Package repositories are just a bunch of .deb files on a server somewhere that apt can download and install for you, if you put the server's URL in the sources.list file or a sources.list.d/<stuff> file.

apt update is used to update the list of available software packages
apt upgrade is used to upgrade the software packages that are already installed with the latest versions that were found by apt update



There are GUIs for apt and dpkg:
for apt: synaptic, muon...
for dpkg: gdebi, dpkg-deb...


/!\ apt and dpkg are not the only package managers in Linux. There are others like rpm, yum, dnf, zypper, pacman, emerge, portage, apk, etc. Each distribution has its own package manager. /!\
On Debian, and Debian-based distributions like Ubuntu, apt and dpkg are the package managers. Don't use multiple package managers, they are not compatible with each other. Use only one package manager for your distribution, or else things will break.

Flatpak and Snap are package managers that containerize software, meaning they put it in big boxes with all their dependencies (software your softawre needs to work) bundled up in a hermetic box. That means you can install software with your package manager as well as flatpak and snap in parallel. Snap is bad, its software is outdated and the updating process is broken. Flatpak is better, but I haven't used it. You can already install every software using only apt and dpkg with .deb files.
It is recommended to use apt and .debs as much as possible.

