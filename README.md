<img width="337" height="109" alt="Azure+ Logo" src="https://github.com/user-attachments/assets/c9ca13ef-3f52-474e-8f57-ee4ac73944af" />

# Azureplus
A Universal packages for Azure Linux 4.0 Based on Fedora 43

Installation

run sudo nano /etc/yum.repos.d/azureplus.repo

then add this

[azureplus]
name=Azureplus
baseurl=https://download.fedoraproject.org/pub/fedora/linux/releases/43/Everything/x86_64/os/
enabled=1
gpgcheck=1
gpgkey=https://fedoraproject.org/fedora.gpg

Alternative: Mirrorlist Method
If you prefer mirrors (recommended for Azure VMs to avoid downtime)

[azureplus]
name=Azureplus
mirrorlist=https://mirrors.fedoraproject.org/mirrorlist?repo=fedora-43&arch=x86_64
enabled=1
gpgcheck=1
gpgkey=https://fedoraproject.org/fedora.gpg

Save the file as /etc/yum.repos.d/azureplus.repo

run
sudo dnf clean all
sudo dnf makecache
