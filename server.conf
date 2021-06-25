#remote 172.19.0.1
port 1200
proto udp
dev tun
#sndbuf 0
#rcvbuf 0
ca ca.crt
cert server.crt
key server.key
dh dh.pem
#tls-auth ta.key 0
topology subnet
mode server 
tls-server
ifconfig 10.8.0.0 255.255.255.0
#ifconfig-pool-persist ipp.txt
push "route-gateway 10.8.0.0"
#push "dhcp-option DNS 8.8.8.8"
#push "dhcp-option DNS 8.8.4.4"
keepalive 10 120
cipher AES-256-CBC
auth SHA256
#user nobody
#group nogroup
persist-key
persist-tun
status openvpn-status.log
verb 4
#crl-verify crl.pem
