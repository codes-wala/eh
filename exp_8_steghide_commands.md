steghide --version

create a folder in downloads. lets name it steg

download an image(here: car.jpeg) from internet
place that image is steg folder

cd Downloads/steg

nano secretinfo.txt
inside type the so called "secret info"

steghide embed -cf car.jpeg -ef secretinfo.txt
enter passphrase: any password

steghide info car.jpeg

steghide extract -sf car.jpeg
press y

cat secretinfo.txt
