# [dockovpn](https://dockovpn.io/)
https://openvpn.net

<pre>
docker run -it --rm --cap-add=NET_ADMIN \
-p 1194:1194/udp -p 80:8080/tcp \
-e HOST_ADDR=$(curl -s https://api.ipify.org) \
--name dockovpn alekslitvinenk/openvpn
</pre>
