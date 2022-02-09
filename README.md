# Ansible: Cisco NX-OS Always On Lab

Ansible `playbook` to interact with a Cisco NX-OS devices, with a pre-configured NX-OS lab device located in the Cisco DevNet `Always On` DevNet infrastructure, defined for you in the `inventory/hosts.yml` file.  Please be courteous to your fellow network automation enthusiasts, and follow the Terms & Conditions Cisco outlines on [DevNet](https://developer.cisco.com) when interacting with the lab.

The purpose of this `playbook` is to get you up and running quickly with Ansible, and the Cisco NX-OS platform via the `cisco.nxos.nxos` Ansible Galaxy Collection.

## Deployment
>The `host_vars` are tailored towards a modern version of Ansible 5.x.x, and the latest version of the `cisco.nxos` collection.  If you are using a different version of Ansible, please review the `host_vars` to ensure compatibility, and consider making use of a python virtual environment (`venv`) when trying out this project.

### You will need to make sure `libssh` is installed on your system or modify the `host_vars`.

- https://www.libssh.org/get-it/
- https://docs.ansible.com/ansible/latest/collections/ansible/netcommon/libssh_connection.html

```bash
apt-get install libssh-dev
```

### Install the Python `requirements.txt` file.

```bash
pip install -r requirements.txt
```

### Make sure you have the `cisco.nxos.nxos` Galaxy Collection.

```bash
ansible-galaxy collection install -r requirements.yml
```

### Run the playbook.

```bash
ansible-playbook -i inventory/hosts.yml site.yml
```

## Authors

- [@netopsengineer](https://www.github.com/netopsengineer)

