# oci-gromacs
### Ansible setup of Gromacs molecular dynamics application

##### Steps:

1. Ensure that the <b>tasks.yaml</b> Ansible playbook file and the <b>hosts</b> inventory file are in the same folder on your machine. You can download them [here](https://github.com/oci-hpc/oci-gromacs/archive/refs/heads/main.zip), and move them to the appropriate machine if necessary with:
<pre>
scp -i &ltpath to your private ssh key&gt tasks.yaml hosts opc@&ltdestination machine ip address&gt:&ltdestination directory&gt
</pre>
2. Edit <b>hosts</b> and replace the IP address placeholder text with the IP address of the destination machine.
<pre>
vi hosts
</pre>
3. Navigate to the directory on your destination machine containing <b>tasks.yaml</b> and <b>hosts</b> and execute the tasks.
<pre>
ansible-playbook -i hosts tasks.yaml
</pre>
4. Ensure that the variable definitions written in <b>/home/opc/.bashrc</b> are set in your environment.
<pre>
source /home/opc/.bashrc
</pre>
5. Validate that the <b>gmx</b> command is now available. Details about the command's usage should be returned as output.
<pre>
gmx
</pre>
