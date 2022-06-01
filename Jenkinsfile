pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
                echo 'Deploying es'
                sh '''
                        #!/bin/bash
                        eval `ssh-agent -s`
                        ssh-add /opt/apps/es.pem
                        ansible-playbook -i hosts infra-common.yml
                         '''
            }
        }
    }
}