pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'docker:dind' 
                }
            }
            steps {
                sh '
                    docker build -t test:0.0.1 .
                '
            }
        }
    }
}