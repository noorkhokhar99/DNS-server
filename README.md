# DNS-server
DNS server




## First, temporarily add a known DNS server to your system.

echo "nameserver 8.8.8.8" | sudo tee /etc/resolv.conf > /dev/null
Then run sudo apt-get update.

If this fixes your temporary resolving messages then either wait for 24 hours to see if your ISP fixes the issue for you (or just contact your ISP) - or you can permanently add a DNS server to your system:

echo "nameserver 8.8.8.8" | sudo tee /etc/resolvconf/resolv.conf.d/base > /dev/null
8.8.8.8 is Google's own DNS server.
