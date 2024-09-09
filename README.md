# ansible-horario-de-verano
Este es un playbook de Ansible para realizar el cambio de hora en Chile de sus switch cisco.

Consiste en dos archivos, el archivo "host" debe estar ubicado en; 

     /etc/ansible/hosts

O lo podría editar y dejer configurado como el archivo de ejemplo.

El archivo host, tiene por objetivo indicar las IP de sus switches cisco, y la credencial con los privilegios suficientes para realizar la modificación necesaria.

El archivo cambia_horario_verano.yml, puede estar en su directorio personal.


Para ejecutar, se debe tener instalado ansible, además de tener ansible-pylibssh;

En linux tipo debian;

     apt install ansible
     apt install python3-pip
     pip install ansible-pylibssh

finalmente, para poder ejecutar el playbook;

     ansible-playbook cambia_horario_verano.yml
