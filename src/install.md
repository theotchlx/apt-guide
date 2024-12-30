# Install stuff

install software from remote repository: (that means it will get updates)
apt install <name>

install software from a .deb file (only one version of the software, no updates unless you set it up)
dpkg -i <name>.deb

apt can actually do dpkg's job and install a .deb file:
apt install ./<name>.deb (notice the ./ to signify it's a file in your current directory, not a name to look up)

