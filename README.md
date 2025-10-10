🔧 Features

Checks available free space in the volume group (VG)

Validates current logical volume (LV) size

Optionally extends the LV and resizes the filesystem

Supports check mode and change mode

Ideal for managing LVM on large-scale bare metal infrastructure

📂 Structure

lvextend.yml – Main Ansible playbook

vault.yml – Optional encrypted variables (e.g., credentials or config)

inventory.txt – Host definitions for bare metal servers

🚀 Usage
ansible-playbook -i inventory.ini lvextend.yml --extra-vars "change_mode=true"

Set change_mode=false for a dry run (default is false).
