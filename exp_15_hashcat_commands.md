echo hello | base64

echo aGVsbG8K | base64 -d

echo -n "hello" | md5sum

echo 5d41402abc4b2a76b9719d911017c592 > hash.txt

ls /usr/share/wordlists/ (check if at this location, rockyou.txt is there. if rockyou.txt.gz is there instead of rockyou.txt then:)

to extract it:
sudo gzip -d /usr/share/wordlists/rockyou.txt.gz

hashcat -m 0 -a 0 hash.txt /usr/share/wordlists/rockyou.txt

hashcat --show -m 0 hash.txt
