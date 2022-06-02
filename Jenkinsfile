pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
                echo 'start'
                sh 'ansible-playbook infra-common.yml -i hosts --private-key /opt/apps/es.pem -u root'
                echo 'suc'
            }
        }
    }
}