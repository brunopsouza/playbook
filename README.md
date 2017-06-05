# ANSIBLE PLAYBOOKS

Instruçoes de instalação para NGINX - PHP 7 - MYSQL.

* Na pasta host se encontra o inventario dos hosts a serem gerenciados.

* Na pasta roles se encontra as estruturas de pastas das tarefas a serem executadas.<br>
- Dentro da pasta de cada tarefa contem a pasta tasks e pode conter a pasta template.<br>
- A pasta task contem o arquivo main.yml que nada mais é a instrução de instalação e cofiguração.<br>
- A pasta template contem os arquivos de configuração a serem copiados para o servidor remoto.
 
* O arquivo server.yml contem a referência das tarefas que estão dentro da pasta roles e ode refereciar um grupo do inventário para executar as tasks.

O comando a ser executado é:

ansible-playbook -i inventario server.yml
