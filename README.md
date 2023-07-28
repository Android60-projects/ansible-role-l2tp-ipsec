# L2TP IPsec Ansible

This directory contains playbooks used for installing L2TP IPsec server using xl2tpd and libreswan packages.

## Install role:
```
ansible-galaxy install git+https://gitlab.myhomelab.xyz/ansible-roles/l2tp-ipsec-ansible.git,,android06.l2tp_ipsec
```

## Tags:
```
- l2tp-config
- l2tp-auth-config
```

## Available variables:
```
openvpn_port: "1194"
openvpn_proto: "udp"
openvpn_easyrsa_path: "/opt/EasyRSA"
openvpn_configuration_directory: "/etc/openvpn/"
easyrsa_version: "3.0.9"
ovpn_admin_path: "/opt/ovpn-admin"
nginx_global_auth_username: "your-username"
nginx_global_auth_password: "your-password"
firewalld_default_interface_zone: "public"
```
