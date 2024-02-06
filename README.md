# vagrant

Install Vagrant and VirtualBox on Fedora

#Step 1: Check CPU Intel VT or AMD-V extensions
$ cat /proc/cpuinfo | egrep "vmx|svm"


sudo dnf install -y wget gcc binutils make glibc-devel patch libgomp glibc-headers  kernel-headers kernel-devel-`uname -r` dkms


sudo dnf install  libQt5Help*


sudo dnf install rpm _from-website.rpm 


sudo usermod -a -G vboxusers ${USER}

$ sudo /usr/lib/virtualbox/vboxdrv.sh setup

vboxdrv.sh: Stopping VirtualBox services.
vboxdrv.sh: Starting VirtualBox services.
vboxdrv.sh: Building VirtualBox kernel modules

cd ~/
VER=$(curl -s https://download.virtualbox.org/virtualbox/LATEST.TXT)
wget https://download.virtualbox.org/virtualbox/$VER/Oracle_VM_VirtualBox_Extension_Pack-$VER.vbox-extpack
double click on extension for install it

===================================
sudo dnf install -y dnf-plugins-core
sudo dnf config-manager --add-repo https://rpm.releases.hashicorp.com/fedora/hashicorp.repo
sudo dnf -y install vagrant


### Other solution
sudo apt install virtualbox-guest-utils virtualbox-guest-dkms
sudo modprobe vboxnetadp
