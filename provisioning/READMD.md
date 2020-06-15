# Provisioning 

Disponibiliza a infraestrutura mínima necessária para um cluster de k8s utilizando o Ansible

## Requisitos

Esse provisionamento está feito pelo ansible na AWS.
Necessário boto3 para sua correta execução.

```bash
sudo easy_install pip
pip install boto3

```

## Usage

```ansible
ansible-playbook -i hosts main.yml
```


## License
[MIT](https://choosealicense.com/licenses/mit/)