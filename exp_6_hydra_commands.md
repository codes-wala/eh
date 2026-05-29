hydra

sudo service ssh start
enter password

sudo service ssh status

sudo adduser testuser
set password
let name and other details be default

nano passwords.txt
add the list of password among which one is the correct password

hydra -l testuser -P passwords.txt ssh://127.0.0.1
