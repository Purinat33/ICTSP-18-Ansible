# Important Commands!

Before we isolate the setup from the internet we need to run: `ansible-playbook -i inventory.ini internet_tasks.yml --vault-password-file .vault_pwd.txt`

After that:
Run: `ansible-playbook -i inventory.ini main.yml --vault-password-file .vault_pwd.txt` or replace `main.yml` with specific playbook `.yml` you want to run

Prerequisite:
1. Every device needs `openssh-client`, `openssh-server` and `python`/`python3` installed
2. The control device (The device running these commands), in addition to having Ansible installed, must give its SSH key to every managed devices:
	* On the control device, perform `ssh-keygen` then `ssh-copy-id user@IP` where `user` is a user on a controlled/managed device and the `IP` is the IP of the same managed device.
	* You should be able to `ssh user@IP` to a managed device without needing to use a password if everything is performed correctly.
