pipeline {
    agent any
    
    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                // Execute the Ansible playbook
                sh 'ansible-playbook -i /home/ec2-user/hosts simple.yml
'
            }
        }
    }
}

