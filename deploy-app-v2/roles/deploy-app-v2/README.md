deploy-app-v2
=========

Deploy de app em utilizando modulo k8s Ansible  com template


Requirements
------------

Cluster de k8s rodando
Arquivo hosts deve ser igual arquivos install_k8s;


Example Playbook
----------------

- hosts: k8s-master
  become: yes
  user: ubuntu
  roles:
  - { role: deploy-app, tags: ["deploy_app_role"]  }

