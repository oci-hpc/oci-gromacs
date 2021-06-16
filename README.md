# oci-gromacs
Ansible setup of Gromacs molecular dynamics application

Usage:

To set up Gromacs on your machine:

1. Ensure that tasks.yaml is on your machine
2. Navigate to the folder containing tasks.yaml and execute the tasks:
<pre>
ansible-playbook -i hosts tasks.yaml
</pre>
3. Ensure that the variable definitions set in /home/opc/.bashrc are set in your environment.
<pre>
source ~/.bashrc
</pre>
