pipeline {
    agent any

    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                script {
                    // Run ansible-playbook command with the inventory file
                    sh 'ansible-playbook -i /home/ec2-user simple.yml'
                }
            }
        }
    }
}
