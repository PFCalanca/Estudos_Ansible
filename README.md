# Estudos_Ansible
<p>
Repositorio de testes e estudos Ansible
</p>
<p align='center'>
<img src="https://github.com/PFCalanca/Estudos_Ansible/blob/master/readme/Ansible_logo.svg.png" width="324" height="324">
</p>

Nesse repositório eu pratiquei a montagem de um playbook, para uma aplicação de 3 camadas
com um banco de dados, uma web server e uma web application funcionar.



## Tecnologias 

Tecnologias usadas.

* Asinble
* MySQL
* PHP
* Wordpress

## Services Used

* Github

## Como fazer substituições para ter uma variável mais replicável?

* Para fazer esse ambiente utilizei a pasta group_vars la temos o file all.yml onde eu como que todas as variáveis, seria uma opção também criar um file separado
  para o server e outro para o banco.

![Homepage image](https://github.com/PFCalanca/Estudos_Ansible/blob/master/readme/var.png)


# Roles

## Por que usar roles?
- Utilizamos os rolês para podermos por exemplo replicar  esse playbook com apenas duas ou adicionar outra com menos dor de cabeça. 
  As roles deixam nosso ambiente mais organizado e replicável.
  
  
![Posts](https://github.com/PFCalanca/Estudos_Ansible/blob/master/readme/Roles.png)

# Função da pasta Tasks:
  - Sabendo que o Ansible entende essa separação das pastas podemos criar uma para Tasks(onde temos toda configuração de instalação e configuração)
  
  
![Posts](https://github.com/PFCalanca/Estudos_Ansible/blob/master/readme/task_mysql.png)

# Função da pasta Handlers:
  - A pasta handlers que tem a função de reiniciar nosso serviço para garantir que a atualização será feita. Se estamos construindo ou fazendo manutenção, utilizar essa “task especial” facilita bastante e pode ser simplesmente chamada ao final da minha task.
    a configuração do handlers é  a main.yml 

![Posts](https://github.com/PFCalanca/Estudos_Ansible/blob/master/readme/handlers.png)


  
## No meu projeto temos 3 roles:
  - MySQL
  - webserver
  - wordpress


### Com toda essa estratégia conseguimos deixar um provisioning.yml bem mais tranquilo de entender.
![Post show](https://github.com/PFCalanca/Estudos_Ansible/blob/master/readme/prov.png)



## Links
  - Repository: https://github.com/PFCalanca/Estudos_Ansible
  - Caso você encontre algum erro de segurança ou algum bug, notifique usando o issue tracker.
## Contato:
  https://www.linkedin.com/in/paulo-de-freitas-calanca-109906174/
