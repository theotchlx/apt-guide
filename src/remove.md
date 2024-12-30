# Remove stuff

apt purge <name> (removes the software and all its configuration files - apt remove doesn't remove the configuration files)
followed by
apt autoremove --purge (removes any dependencies that are no longer needed)

or apt purge --autoremove?


Remove software that was installed from a .deb file:
dpkg -r <name>

