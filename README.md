# wp-emerson

# Instalando wordpress com ansible

## Utilizado CentOS 7 ##

# Instale ansible 

#yum install ansible -y

No diretorio /etc/ansible faça o clone do repositorio, diretorios /playbooks e /roles mantenha na raiz do diretorio, a instalacao foi feita em localhost edite o arquivo de inventorio hosts, caso precise adicionar novos hosts siga este modelo. 

#vim hosts

[wordpress]

127.0.0.1

# Para testar comunicacao do host

#ansible localhost -c local -m ping

## Executar o arquivo #playbook.yml que se encontra no diretorio /playbooks

#ansible-playbook -c local playbooks/playbook.yml
