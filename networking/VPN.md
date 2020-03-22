# VPN

## Recipes

- Setup your own free OpenVPN on AWS EC2:

  - [Setup OpenVPN with CentOS and AWS EC2](https://www.itsfullofstars.de/2018/04/setup-openvpn-server-on-amazon-ec2/)
  - [Setup OpenVPN with Ubuntu 16.04](https://www.digitalocean.com/community/tutorials/how-to-set-up-an-openvpn-server-on-ubuntu-16-04)

You might need to [add custom DNS] on the client machine

[add custom DNS]: https://tunnelblick.org/cConnectedBut.html#how-to-use-a-different-dns-server

If you can connect succefully, but don't have Internet, try running this:

```bash
sudo iptables -t nat -A POSTROUTING -s 10.8.0.0/24 -o eth0 -j MASQUERADE
```
