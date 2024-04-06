# Nix-ProtonVPN

Basic and simple bash script for controlling OpenVPN connections on Nix (can be used on any system) due to the offical ProtonVPN app being broken and support is terrible. This script will disable ipv6 before connecting to VPN server, then enable it after disconnecting, this prevents ipv6 leaks and protonVPN does not support ipv6 connections. I used .bashrc to add a terminal command and run the script by typing vpn to make it as simple and quick as possible. e.g (alias vpn='bash /home/YOURNAME/bin/vpn.sh').

You may need to change your primary connection type at the start of the code, currently its set to find active wifi connection. You may want ethernet for example if using a wired connection. primary_connection=$(nmcli connection show --active | grep wifi | awk '{print $1}')

May add more options/features in the future. This is just a hacky workaround for my own use.
