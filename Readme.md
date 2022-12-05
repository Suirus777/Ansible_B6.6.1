<center><h2><b>Skillfactory: Module 6 - Ansible!!!! </center></h2></b><br><br>

<h3><b>Задание B6.6.1</h3><b> <br>
<br>
Создайте Ansible-роль, устанавливающую и запускающую FTP-сервер vsftpd. <br>
<br>
Ответ: <br>
1. Командрой <b> ansible-galaxy init vsftpd </b> была создана роль. <br>
2. В <b> /roles/vsftpd/tasks/main.yml </b> был добавлен код для установки <b> vsftpd сервера </b> <br>
3. Был создан шаблон <b> /roles/vsftpd/templates/vsftpd.j2 </b> для vsftpd.conf    <br>
4. Был создан <b> vsftpd.yml </b> с установкой роли ftp сервера <br>
5. Результат: ftp сервер работает по локальным пользвотелям сервера. <br>
  <b>  odmin@devops1:~$ ps aux | grep vsftpd <br>
root      111092  0.0  0.2   6808  2968 ?        Ss   18:08   0:00 /usr/sbin/vsftpd /etc/vsftpd.conf <br>
odmin     111311  0.0  0.0   6432   656 pts/0    S+   18:25   0:00 grep --color=auto vsftpd <br>
odmin@devops1:~$ </b> <br>
   
