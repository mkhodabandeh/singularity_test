bootstrap:docker
From:ubuntu:latest

%runscript

echo "This gets run when you run the image!" cd /code exec echo "Hello" "$@"

%post

echo "This section happens once after bootstrap to build the image."
mkdir -p /code
apt-get update
apt-get install vim
echo "Kibbles and bits, but really more bits."

echo "Installing pip"
apt-get install python-pip python-dev build-essential 
pip install --upgrade pip
pip install --upgrade virtualenv
echo "Installation done for pip"
