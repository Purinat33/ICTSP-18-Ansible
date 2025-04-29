# Important Commands!

Before we isolate the setup from the internet we need to run: `ansible-playbook -i inventory.ini internet_tasks.yml --vault-password-file .vault_pwd.txt`

After that:
Run: `ansible-playbook -i inventory.ini main.yml --vault-password-file .vault_pwd.txt`

or replace `main.yml` with specific playbook `.yml` you want to run

Prerequisite:
1. Every device needs `openssh-client`, `openssh-server` and `python`/`python3` installed
2. The control device (The device running these commands) must give its SSH key to every managed devices.
	* `ssh-keygen` then `ssh-copy-id user@IP`
	* You should be able to `ssh user@IP` without needing to use a password


ISSUE:
1. ChatGPT suddenly decided to become stupid and refused to answer questions related to server cluster. So now the only manual part as of right now is:
	* You need to edit `/var/ossec/etc/ossec.conf` of server nodes to make a cluster.
	* Everything else, including load balancing logic should already be handled.

2. Accidentally committed .venv/ so now the repo is heavy
