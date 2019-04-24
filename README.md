# Ansible Playbook for Raspbian GNU/Linux 9.8 (stretch)

## Usage

- `ansible-galaxy install --role-file provision/requirements.yml --roles-path provision/roles`
- `ansible-playbook -i provision/inventory/production provision/playbook.yml -b -K`
- `ansible-playbook -i provision/inventory/production provision/zabbix-install.yml -b -K`
- `ansible-playbook -i provision/inventory/production provision/zabbix-api-setup.yml -b -K`
- `ansible-playbook -i provision/inventory/production provision/zabbix-group.yml`
- `ansible-playbook -i provision/inventory/production provision/zabbix-template-cert.yml`
- `ansible-playbook -i provision/inventory/production provision/zabbix-template-nasne.yml`
- `ansible-playbook -i provision/inventory/production provision/zabbix-template-openvpn.yml`
- `ansible-playbook -i provision/inventory/production provision/zabbix-host.yml`
- `ansible-playbook -i provision/inventory/production provision/zabbix-hostmacro.yml`
- `ansible-playbook -i provision/inventory/production provision/zabbix-nasne.yml -b -K`
- `ansible-playbook -i provision/inventory/production provision/zabbix-bluetooth-setup.yml -b -K`
- `ansible-playbook -i provision/inventory/production provision/zabbix-bluetooth.yml`

## Development

- `dotenv vagrant up`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-install.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-api-setup.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-group.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-template-cert.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-template-nasne.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-template-openvpn.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-host.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-hostmacro.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-nasne.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-bluetooth-setup.yml vagrant provision`
- `env ANSIBLE_PLAYBOOK=provision/zabbix-bluetooth.yml vagrant provision`
