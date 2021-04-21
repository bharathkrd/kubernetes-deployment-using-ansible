# ansible-k8s-setup
This will setup a kubernetes cluster on Centos7 machines using ansible.
You need these machines:
1. Ansible controller - controller.example.com - 10.0.0.99 - 1 vcpu / 2 gib ram
2. Kubernetes Master - master.example.com - 10.0.0.100 - 2 vcpu / 4 gib ram
3. Kubernetes Node1 - nodeone.example.com - 10.0.0.1 - 1 vcpu / 4 gib ram
4. Kubernetes Node2 - nodetwo.example.com - 10.0.0.2 - 1 vcpu / 4 gib ram

If you can allocate more compute resources, its better
If you change your machine IP's then you have to change those whereever
those were referred.


Requirements
------------
Tested on 
VMware workstation: 16.0
OS version: CentOS: 7.9.2009
Ansible version: 2.9.18
Python : 2.7.5
Kubernetes: 
Number of available CPU: 2

Dependencies
------------
firewall service to be disabled
Disable swap and in fstab
Docker to be installed.
ensure net.bridge.bridge-nf-call-ip6tables is set to 1
ensure net.bridge.bridge-nf-call-iptables is set to 1
Yum: To install the Kubernetes Package
baseurl: https://packages.cloud.google.com/yum/repos/kubernetes-el7-x86_64
gpgkey: https://packages.cloud.google.com/yum/doc/yum-key.gpg https://packages.cloud.google.com/yum/doc/rpm-package-key.gpg




