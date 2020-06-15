Cria instancia para k8s
=========
Será criada as instâncias necessárias para um cluster k8s


Requirements
------------

Nessário boto3 para interação com a AWS.

Role Variables
--------------

Necessário definir as variáveis da AWS com tipo de instância, grupo, imagem e key pair etc.



Example Playbook
----------------

  - hosts: local
    roles:
    - criando-instancias
