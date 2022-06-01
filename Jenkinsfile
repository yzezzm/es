pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
                echo 'Deploying es'
                sh 'cat /opt/apps/es.pem'
                sh 'ssh-agent bash; ssh-add /opt/apps/es.pem ; ansible-playbook -i hosts infra-common.yml'
            }
        }
    }
}