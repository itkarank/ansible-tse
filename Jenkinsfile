pipeline {
    agent any

    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                script {
                    // Run ansible-playbook command with the inventory file
                    
                    sh'ansiblePlaybook inventory: '/var/lib/jenkins/workspace/testing ansible/hosts', playbook: '/var/lib/jenkins/workspace/testing ansible/simple.yml'
                }
            }
        }
    }
}
