# automate_patching_ansible
A repo to automate ansible patching - DEMO

This repo has a working automated patching role with playbook to display how easily machines can be patched depending on the variables passed to tower. It also has a ping all hosts playbook that can be added as a first step in a workflow to show how patching can be automated and included within a workflow template. 

If you are running this against the latest rhpds instances it won't actually change anything. To show its utility I log into one of the end points and do the following: 

1. yum remove tuned
2. yum install tuned-2.14.0-3.el8

This then lets the patching role install the latest version on whichever node. 
