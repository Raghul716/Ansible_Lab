# Update System: Ensures that the system is updated before the installation.
# Install Required Packages: Installs necessary packages (wget, gnupg2, lsb-release, etc.) to add the Veeam repository and manage it.
# Add Veeam Repository: Adds the official Veeam repository for both Debian and RHEL-based systems.
# Install Veeam Agent: Installs the Veeam Agent package from the added repository.
# Enable and Start Veeam Service: After installation, it enables and starts the veeamservice.
# Confirm Installation: Verifies the installation by checking the installed Veeam Agent version and outputs the result.

Run the playbook
ansible-playbook -i inventory_file linux.yml
