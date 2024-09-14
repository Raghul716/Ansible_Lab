# FOR LINUX DISTRIBUTION

 Update System: Ensures that the system is updated before the installation.
 
 Install Required Packages: Installs necessary packages (wget, gnupg2, lsb-release, etc.) to add the Veeam repository and manage it.
 
 Add Veeam Repository: Adds the official Veeam repository for both Debian and RHEL-based systems.
 
 Install Veeam Agent: Installs the Veeam Agent package from the added repository.
 
 Enable and Start Veeam Service: After installation, it enables and starts the veeamservice.
 
 Confirm Installation: Verifies the installation by checking the installed Veeam Agent version and outputs the result.

Run the playbook
ansible-playbook -i inventory_file linux.yml


# FOR WINDOWS MACHINES

Download Installer (win_get_url):

Downloads the Veeam Agent for Windows installer from the official Veeam website to the C:\temp directory.
You can replace the url value with the latest version or another download link if necessary.
Install Veeam Agent (win_package):

Uses the win_package module to install the Veeam Agent silently.
The product_id corresponds to the Veeam Agent's GUID. This can vary by version, so it's best to check the specific product ID using tools like Get-WmiObject or via the Windows registry for the version you're installing.
Ensure the Service is Running (win_service):

Ensures that the VeeamEndpointBackupSvc service (the Veeam Agent service) is running and is set to start automatically.
Verify Installation (win_shell):

Uses a PowerShell command to check if the Veeam Agent is installed by querying the Win32_Product class.
The debug task outputs the installed version of Veeam Agent to verify successful deployment.
