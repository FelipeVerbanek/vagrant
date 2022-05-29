
Projeto criado para estudo, onde utiliza algumas tecnologias como Vagrant, Puppet e Ansible.
O objetivo do projeto é subir algumas maquinas virtuais, com um servidor mysql e um servidor php.

# Vagrant


* Iniciar maquinas virturais
```
vagrant up
```
* Parando maquinas virtuais
```
vagrant halt
```
* Excluindo maquinas
```
vagrant destroy
```

# Criando chave SSH
* Exemplo:
```
 ssh-keygen -t rsa
```
Coloque a chave privada no diretorio bionic com o nome id_bionic, e a chave pública dentro do diretorio bionic/configs.

* Conectando na maquina via ssh:
```
vagrant ssh
```

# Utilizando Ansible

Realize a conexão ssh na maquina "ansible", exemplo:
```
vagrant ssh ansible
```

Execute: 
```
ansible-playbook -i /vagrant/configs/ansible/hosts /vagrant/configs/ansible/playbook.yml
```