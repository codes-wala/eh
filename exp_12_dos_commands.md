sudo wireshark

Loopback: lo

start capturing

on new terminal tab:
sudo apt install hping3 -y

sudo ping -f 127.0.0.1 (dos attack)

sudo hping3 -S --flood -V 127.0.0.1 (syn flood)

stop the capture

filter icmp

filter tcp.flags.syn==1 & check flags by clicking on:
src:......,dst....
