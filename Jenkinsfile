pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
                echo 'Deploying es'
                cat /opt/apps/es.pem
                sh 'ansible-playbook -i hosts infra-common.yml'
            }
        }
    }
}