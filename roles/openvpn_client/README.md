Role Name
=========

Установка openvpn-client

Requirements
------------

Ansible >=2.4
Ubuntu 16.04


Role Variables
--------------

Переменые по умолчанию roles/openvpn_client/defaults/main.yml:
 - openvpn_dev_type default  tun (tap or tun)
 - openvpn_tcp_or_udp default udp (tcp or udp)
 - openvpn_remote_server_ip default 8.8.8.8 (remote server IP)
 - openvpn_remote_server_port default 2195  (remote server port)
 - openvpn_package_version default 2.3.10-1ubuntu2.1 (Openvpn version package)

Внутрениие переменные roles/openvpn_client/vars/main.yml:
 - openvpn_user_ca CA сертификат 
 - openvpn_user_tls_auth TLS static key v1
 - openvpn_user_cert Сертификат
 - openvpn_user_key Ключ
 - openvpn_cache_valid_time 86400 (apt cache valid time in seconds)


Dependencies
------------


Example Playbook
----------------


    - hosts: openvpn
      roles:
         - role: openvpn_client

Author Information
------------------
test_example from install openvpn_client
