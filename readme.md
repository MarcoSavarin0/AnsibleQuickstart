### Ansible Quickstart para instancias de EC2

#### Instalación

1. Instalar Ansible

    ```
    sudo apt-get install ansible
    ```

2. Crear el archivo de configuración de Ansible

    ```
    sudo nano /etc/ansible/hosts
    ```

3. Añadir los hosts a la configuración de Ansible

    ```
    ansible_host: xx.xx.xx.xx ip publica de la instancia (pueden ser dos o mas)
    ```

4. Obtener archivo pem de la instancia


5. Ejecutar ping de la instancia

    ```
    ansible-playbook -i host.yml ping.yml 
    ```
    o
    ```
    ansible all -i host.yml -m ping -vvv
    ```

6. Ejecutar el set up de la instancia

    ```
    ansible-playbook -i host.yml apache_setup.yml
    ```


