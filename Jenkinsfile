pipeline {
    agent any

    stages {
        stage('Deploy Ansible Playbook') {
            steps {
                script {
                    

                    // Run ansible-playbook command with the inventory file
                    sh "ansible-playbook -i hosts simple.yml
                }
            }
        }
    }
}
