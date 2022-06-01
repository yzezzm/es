pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
               ansiblePlaybook(
                credentialsId: 'ess',
                inventory: 'hosts',
                playbook: 'infra-common.yml'
               )
            }
        }
    }
}