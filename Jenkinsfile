pipeline {
    agent any

    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                script {
                    // Set the path to the private key file
                    def privateKeyPath = '/var/lib/jenkins/workspace/testing ansible/newkey.pem'

                    // Set proper permissions on the private key file
                    sh "sudo chmod 400 ${privateKeyPath}"

                    // Run ansible-playbook command with the inventory file
                    sh "ansible-playbook -i '/var/lib/jenkins/workspace/testing ansible/hosts' '/var/lib/jenkins/workspace/testing ansible/simple.yml'"
                }
            }
        }
    }
}
