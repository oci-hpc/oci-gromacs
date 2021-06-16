# oci-gromacs
### Ansible setup of Gromacs molecular dynamics application

Usage:

To set up Gromacs on your machine:

1. Ensure that <b>tasks.yaml</b> is on your machine. You can download it [here](https://github.com/oci-hpc/oci-gromacs/archive/refs/heads/main.zip), and move it to the appropriate machine if necessary with:
<pre>
scp -i PATH_TO_YOUR_PRIVATE_SSH_KEY tasks.yaml opc@IP_ADDRESS:DESTINATION_DIRECTORY
</pre>
3. Navigate to the folder containing tasks.yaml and execute the tasks:
<pre>
ansible-playbook -i hosts tasks.yaml
</pre>
3. Ensure that the variable definitions set in /home/opc/.bashrc are set in your environment.
<pre>
source ~/.bashrc
</pre>
