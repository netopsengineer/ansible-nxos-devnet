# Cisco NX-OS Always On Lab

Playbook to interact with NX-OS devices


## Deployment

### You will need to make sure `libssh` is installed.

- https://www.libssh.org/get-it/

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

### Run the playbook..

```bash
ansible-playbook -i inventory/hosts.yml site.yml
```

## Authors

- [@netopsengineer](https://www.github.com/netopsengineer)

