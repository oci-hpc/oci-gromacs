# oci-gromacs
### Ansible setup of Gromacs molecular dynamics application

Steps:

1. Ensure that <b>tasks.yaml</b> is on your machine. You can download it [here](https://github.com/oci-hpc/oci-gromacs/archive/refs/heads/main.zip), and move it to the appropriate machine if necessary with:
<pre>
scp -i <path to your private ssh key> tasks.yaml opc@<destination machine ip address>:<destination directory>
</pre>
2. Navigate to the directory on your destination machine containing <b>tasks.yaml</b> and execute the tasks:
<pre>
ansible-playbook -i hosts tasks.yaml
</pre>
3. Ensure that the variable definitions set in /home/opc/.bashrc are set in your environment.
<pre>
source ~/.bashrc
</pre>
