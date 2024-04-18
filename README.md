# ansible_role_focalboard
Ansible Playbook para configurar focalboard para project management.

Testeado con Vagrant + qemu + ubuntu_20.04 + ansible_2.15

---

### Descripción

La idea del proyecto es automatizar vía ansible la instalación de [focalboard](https://github.com/mattermost/focalboard) para pruebas de laboratorio, el repo cuenta con 3 roles:

1. focalboard
2. mysql
3. nginx

### Dependencias

* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)
* [Vagrant](https://developer.hashicorp.com/vagrant/install) (opcional)

### Uso

```
git clone https://github.com/pgraffigna/ansible_role_focalboard.git
cd ansible_role_focalboard
ansible-playbook main.yml
```

### Extras

* Archivo de configuración (Vagrantfile) para desplegar una VM descartable con ubuntu-22.04 con libvirt como hipervisor.
* config.json
* focalboard.service
* focalboard.conf

---
### Uso Vagrant
```
vagrant up
vagrant ssh
```