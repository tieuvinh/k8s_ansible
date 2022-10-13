# k8s_ansible
# Tat SELinux
```
sudo setenforce 0

sudo sed -i --follow-symlinks 's/^SELINUX=enforcing/SELINUX=disabled/' /etc/sysconfig/selinux
```
# Tat swap
```
sudo sed -i '/swap/d' /etc/fstab

  sudo swapoff -a
```

# Thay hostname
Trên node master

`sudo hostnamectl set-hostname master`

Trên node worker

`sudo hostnamectl set-hostname worker1`
