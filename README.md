Role Name
=========

This role installs [minikube](https://minikube.sigs.k8s.io/docs/)

Requirements
------------

The minikube documentation [outlines](https://minikube.sigs.k8s.io/docs/start/#what-youll-need) the requirements needed

Role Variables
--------------

- `minikube_download_url`: <https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64>
- `minikube_install_location`: "{{ ansible_env.HOME }}/.local/bin"
- `minikube_install_location_mode`: 0750
- `minikube_binary`: "{{ minikube_install_location }}/minikube"
- `minikube_binary_mode`: 0750

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: markcaudill.minikube }

License
-------

MIT

Author Information
------------------

