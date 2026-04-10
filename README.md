# ansible-esxi
1 Encrypt the vault:
 ansible-vault encrypt ansible-esxi/group_vars/esxi/vault.yml
2 Update vault_esxi_password with your real ESXi password.
3 Install dependencies:
 pip install pyvmomi
 ansible-galaxy collection install community.vmware
4 Run:
 ansible-playbook -i inventory/hosts playbooks/deploy.yml --ask-vault-pass
