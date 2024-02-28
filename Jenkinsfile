pipeline {
    agent any
    
    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                // Execute the Ansible playbook
                sh 'ansible-playbook -i inventory simple.yml'
            }
        }
    }
}

