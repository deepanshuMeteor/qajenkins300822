pipeline{
        agent any
    stages {
        stage('Test') {
            steps {
                sh 'sudo docker-compose pull && sudo -E DB_PASSWORD=${DB_PASSWORD} docker-compose up -d'
            }
        }
    }
}
