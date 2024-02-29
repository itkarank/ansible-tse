pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                withCredentials([sshUserPrivateKey(credentialsId: ' 35cb42c3-1ab4-482b-a327-b2cb3507b7c0', keyFileVariable: 'SSH_KEY')]) {
                    sh 'ansible-playbook -i hosts --private-key=$SSH_KEY your-playbook.yml'
                }
            }
        }
    }
}

