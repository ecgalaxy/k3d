ECGALAXY k3d
===============

Ansible role that installs [k3d](https://k3d.io/).

K3d is a lightweight wrapper to run k3s (Rancher Lab's minimal Kubernetes distribution) in docker.

Requirements
------------

K3d requires Docker or Podman.

Docker can be installed via `ecgalaxy.docker` ansible role.

Role Variables
--------------

The role has the following variables:

- `k3d_version`: Specify the version of k3d you want to install.
- `k3d_checksum`: Specify the checksum of the k3d version you want to install.
- `k3d_download_url`: Specify the URL to download the k3d binary for the specified version.
- `k3d_installation_dir`: Specify the installation directory for k3d.

Each of these variables has a default value, which can be found in `defaults/main.yml`.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: all
      roles:
        #- ecgalaxy.docker (uncomment to install Docker)
        - ecgalaxy.k3d

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.
