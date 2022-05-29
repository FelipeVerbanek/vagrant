
Projeto criado para estudo, onde utiliza algumas tecnologias como Vagrant, Puppet e Ansible.
O objetivo do projeto é subir algumas maquinas virtuais, com um servidor mysql e um servidor php.

# Criando chave SSH
* Exemplo:
```
 ssh-keygen -t rsa
```
Coloque a chave privada no diretorio bionic com o nome id_bionic, e a chave pública dentro do diretorio bionic/configs.

# Vagrant

Primeiramente acesse o diretório "bionic".

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
* Verificar status das maquinas:
```
vagrant status
```
* Conectando na maquina via ssh:
```
vagrant ssh nome_da_maquina
```

* Para testar acesse:
```
http://localhost:8888/
```
Deve aparecer algo como:
```
Testando conexao

Conectado com sucesso
```