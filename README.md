Role Name
=========

Установка openvpn-client

Requirements
------------


Role Variables
--------------

Переменые по умолчанию roles/openvpn/defaults/main.yml:
 - openvpn_dev_type tun (tap or tun)
 - openvpn_tcp_or_udp udp (tcp or udp)
 - openvpn_remote_server_ip 8.8.8.8 (remote server IP)
 - openvpn_remote_server_port 2195  (remote server port)
 - openvpn_package_version 2.3.10-1ubuntu2.1 (Openvpn version package)
 - openvpn_cache_valid_time 86400 (apt cache valid time in seconds)

Внутрениие переменные roles/openvpn/vars/cert.yml:
 - openvpn_user_ca CA сертификат 
 - openvpn_user_tls_auth TLS static key v1
 - openvpn_user_cert Сертификат
 - openvpn_user_key Ключ


Dependencies
------------


Example Playbook
----------------


    - hosts: openvpn
      roles:
         - role: openvpn

Author Information
------------------
test_example from install openvpn_client
