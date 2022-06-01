pipeline {
    agent any
    stages {
        stage('Deploy to es'){
            steps {
               ansiblePlayBook(
                credentialsId: 'es',
                inventory: 'hosts',
                playbook: 'infra-common.yml'
               )
            }
        }
    }
}