# Linux-NetSpeed



sudo rpm --import https://www.elrepo.org/RPM-GPG-KEY-elrepo.org
sudo rpm -Uvh https://www.elrepo.org/elrepo-release-7.0-4.el7.elrepo.noarch.rpm
sudo yum --enablerepo=elrepo-kernel install kernel-ml -y
sudo egrep ^menuentry /etc/grub2.cfg | cut -f 2 -d \'




	elrepo-release-7.0-4.el7.elrepo.noarch.rpm
