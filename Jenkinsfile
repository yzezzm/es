pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
               ansiblePlaybook(
                       playbook: 'infra-common.yml',
                       inventory: 'host',
                       credentialsId: 'sample-ssh-key')
            }
        }
    }
}