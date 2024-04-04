# Nix-ProtonVPN

Basic and simple bash script for controlling OpenVPN connections on NIX due to the offical ProtonVPN app being broken and support is terrible. This script will disable ipv6 before connecting to VPN server, then enable it after disconnecting, this prevents ipv6 leaks and protonVPN does not support ipv6 connections. I used .bashrc to add the a terminal command and run the script by typing vpn to make it as simple and quick as possible. e.g (alias vpn='bash /home/YOURNAME/Documents/bin/vpn.sh').

You will need to have already imported your openvpn settings and replace the server names to match what you have used. Including your main network connection id.

Will possibly add support for importing vpn server files. This is just a hacky workaround for my own use.
