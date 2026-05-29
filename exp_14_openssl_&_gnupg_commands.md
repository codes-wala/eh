openssl:

nano tops.txt

cat tops.txt

openssl enc -aes-256-cbc -salt -in tops.txt -out tops.enc

cat tops.enc

openssl enc -aes-256-cbc -d -in tops.enc -out decrypt.txt

cat decrypt.txt


gnupg:

nano test

cat test

gpg -c test

ls (to see if test and test.gpg is there)

cat test.gpg

gpg -d test.gpg

