pipeline {
    agent any

    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                script {
                    // Run ansible-playbook command with the inventory file
                   sh 'ansible-playbook -i /var/lib/jenkins/workspace/testing/simple.yml'

                }
            }
        }
    }
}
