# Ansible

Neste repositório estão disponíveis os códigos para alteração de IP e instalação do agente do Zabbix em um servidor Linux.

<strong>Alteração de IP</strong>
O arquivo para alteração do IP está no diretório <em>/Linux/roles/changes/CHANGE_IP.yml</em>
Neste código, irá executar:
  - A alteração do nome do arquivo para .old
  - Em seguida, será criado um novo arquivo de configuração
  - E, por fim, o mesmo será populado com as informações da interface de rede

<strong>Instalação Zabbix Agent</strong>
O script para instalação está no diretório <em>/Linux/roles/zabbix/ZABBIX.yml</em>
Neste código, será feito:
  - O download do instalador do agente
  - Após isso, será feito a atualização dos pacotes do Linux e a instalação do agente.
  - Ao final do processo, o arquivo .conf será previamente configurado de acordo com as informações do servidor do zabbix.
  

<strong>FONTES UTILIZADAS</strong>

- ENTENDER A ESTRUTURA DO ANSIBLE<br/>
https://blog.fabricads.com.br/automacao-com-ansible/#:~:text=%C3%89%20interessante%20comentar%20que%20a,itens%20nos%20t%C3%B3picos%20a%20seguir.
https://www.youtube.com/watch?v=BYM6tqn2UvQ
<br/><br/>
- EXECUTAR COMANDOS NO SCRIPT<br/>
https://docs.ansible.com/ansible/2.8/modules/shell_module.html#shell-module
<br/><br/>
- COMO CRIAR UM ARQUIVO<br/>
https://phoenixnap.com/kb/ansible-create-file
<br/><br/>
- INSERIR VÁRIAS LINHAS EM UM ARQUIVO<br/>
https://www.edureka.co/community/85271/how-to-add-multiple-lines-in-a-file-using-ansible-playbook
https://docs.ansible.com/ansible/2.4/lineinfile_module.html
https://docs.ansible.com/ansible/latest/collections/ansible/builtin/lineinfile_module.html
<br/><br/>
- ALTERAR VÁRIAS LINHAS EM UM ARQUIVO COM O REGEX
https://www.middlewareinventory.com/blog/ansible-lineinfile-multiple-lines-replace-multiple-lines/
