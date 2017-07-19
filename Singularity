bootstrap:docker
From:nvidia/cuda:8.0-cudnn5-devel-ubuntu16.04

%environment
MEHRAN=True
export $MEHRAN

%runscript

echo "This gets run when you run the image!" cd /code exec echo "Hello" "$@"

%post

echo "This section happens once after bootstrap to build the image."
apt-get install vim
echo "Kibbles and bits, but really more bits."

echo "Installing pip"
apt-get install build-essential python python-pip python-dev  
pip install --upgrade pip
pip install --upgrade virtualenv
echo "Installation done for pip"
