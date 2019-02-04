# Despliegue de Drupal con Ansible

Este escenario contiene dos máquinas, nodo 1 y nodo2. Cada una tendrá diferentes servicios instalados:

- nodo1: Base de datos PostgreSQL y DNS bind9
- nodo2: Servidor web Apache con mod-php corriendo Drupal

Para levantar el escenario, ejecutaremos:
```
vagrant up
```
Acto seguido, para ejecutar el _playbook_, introduciremos el siguiente comando:
```
ansible-playbook site.yml
``` 
Una vez hecho esto, configuraremos como DNS primario la dirección IP de nodo1 (10.0.0.10) y podremos acceder al sitio Drupal creado (credenciales -> user: admin, pass:admin) desde drupal.example.org
