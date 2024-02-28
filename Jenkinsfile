pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout your Ansible playbook repository
                git 'https://github.com/itkarank/ansible-tse.git'
            }
        }
        stage('Deploy Ansible Playbook') {
            steps {
                // Execute the Ansible playbook
                sh 'ansible-playbook -i inventory simple.yml'
            }
        }
    }
}

