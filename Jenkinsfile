pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
                echo 'Deploying es'
                sh '''
                        #!/bin/bash
                        ssh-agent bash; ssh-add /opt/apps/es.pem
                         '''
                sh 'ansible-playbook -i hosts infra-common.yml'
            }
        }
    }
}