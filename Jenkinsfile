pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
                ansiblePlaybook(
                               playbook: 'infra-common.yml',
                               inventory: 'hosts',
                               credentialsId: 'ess')
            }
        }
    }
}