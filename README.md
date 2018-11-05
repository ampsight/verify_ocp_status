# verify_ocp_status
Verify status of OpenShift 3.x. This is a subset of the Red Hat [Odie](https://github.com/RedHatOfficial/odie) project.  

OCP Health check documentation [OCP Health Checks](https://docs.openshift.com/container-platform/3.11/day_two_guide/environment_health_checks.html)  


To use, you need at least the masters group defined in an ansible hosts file like so:  
```
[masters]
ocp-master-[01:03].ocp.example.com
```

Execute the playbook:
```
$ansible-playbook -i <your_inventory_file> verify_ocp.yml
```
