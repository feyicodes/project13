## ANSIBLE DYNAMIC ASSIGNMENTS AND COMMUNITY ROLE

Dynamic assignments are different from static assignments by the use of "include" moodule instead of "import" module. The main difference is that static assignment statements are pre-processed at the time playbooks are parsed, while dynamic assignment statements are only processed during the execution of the playbook. Hence, ansible processes all playbooks referenced during the time it is parsing the statement in static assignment while for dynamic assignment, after parsing statements the changes to statements encountered during execution will be utilized.

The advantage offered by dynamic assignment is its use for specific variables, while its demerit is difficulty to debug due to its dynamic nature.

Firstly, I created a new folder on the home directory of the Jenkins instance and cloned the ansible-congfig repo on github in order to replicate project 12. I did this because I had challenges accessing the Jenkins instance via Virtual Studio Code using SSH. I experienced a lot of SSH connection failures that my initial jenkins instance was no longer reachable via SSH but only through the CLI on AWS website.    