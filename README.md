# Projeto-k8s-cluster (Treinamento Descomplicando Ansible)

Através do Ansible será realizado:
- Criação de instancia AWS;
- Criação de um cluster Kubernetes usando as instâncias criadas anteriormente;
- Deploy app com Ansible;
- Deploy app com modulo Kubernetes;

## Requerimento

Ansible e boto3 para AWS: 
- docs.ansible.com/ansible/latest/installation_guide/intro_installation.html
```bash
sudo apt update
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```
```bash
sudo easy_install pip
pip install boto3
```
Configurando ambiente aws
```
export AWS_ACCESS_KEY_ID='AK123'
export AWS_SECRET_ACCESS_KEY='abc123'
```

## Modo de uso

Provisionar as máquinas utilizando o Ansible e o conteúdo Provisioning

```Ansible
rm hosts
cp hosts_empty hosts
ansible-playbook -i hosts main.yml
```
- Importa a "pem" utilizadas para criar as máquinas (necessário para instalação do kubernetes):
```bash
ssh-agent bash
ssh-add key.pem
````

Utilizar o playbook install_k8s e deploys, mais informações visualizar Readme nos diretórios respectivos.


## Contribuição 
https://www.linuxtips.io/

## License
[MIT](https://choosealicense.com/licenses/mit/)
