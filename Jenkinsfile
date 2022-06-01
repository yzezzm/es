pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
               ansiblePlaybook(
                credentialsId: 'es',
                inventory: 'hosts',
                playbook: 'infra-common.yml'
               )
            }
        }
    }
}