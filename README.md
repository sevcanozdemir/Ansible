# Ansible

ansible-playbook all -m ping 

ansible-playbook -a "uptime" all

ansible-galaxy collection install ansible.posix  --Install additional Ansible collection for firewalld


https://docs.ansible.com/ansible/2.9/modules/

--crontab
*/3 * * * * /usr/bin/ansible-playbook /etc/ansible/playbooks/copy.yml -i /etc/ansible/playbooks/invIp

*/3 * * * * /ansible/projects/sunucubilgileri/server_info.yml -i /ansible/sunuculist/playbooks/invncpa
- name: create file with a date in name
  file: path="/path/somefile{{ lookup('pipe', 'date +%Y%m%d-%H%M') }}"


--start-at-task 'Task name'  --> task başlangıcını atıyoruz
--extra-vars password=passwd123  --> değişkeni komuttan girmek istiyorsak
 

 ansible.builtin.shell  --> modulünün çalışması için python3.9 'a ihtiyaç vardır.
sudo apt update
sudo apt install python3.9