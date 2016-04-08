Jenkins Job DSL Pipelines Framework Ansible Role
================================================

Ansible role that aids in setting up Jenkins pipelines using
https://github.com/kahowell/jenkins-job-dsl-pipelines.

Usage
-----
If you've never used ansible before, you can do something like follows:

    mkdir roles
    echo $JENKINS_HOST > inventory
    git clone https://github.com/kahowell/jenkins-job-dsl-pipelines-ansible roles/jenkins_pipelines
    cat > site.yml <<EOF
    ---
    - hosts: all
      roles:
        - jenkins_pipelines
    EOF
    ansible-playbook -i inventory site.yml

License
-------
AGPLv3; see LICENSE.txt
