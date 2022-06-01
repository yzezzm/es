pipeline {
    stages {
        stage('Deploy to es'){
            steps {
                echo 'Deploying es'
                sh 'ansible-playbook -i hosts infra-common.yml'
            }
        }
    }
}