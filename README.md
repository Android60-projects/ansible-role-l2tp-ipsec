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
firewalld_default_interface_zone: "public"
```
