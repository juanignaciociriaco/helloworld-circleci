pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:3-alpine' 
                }
            }
            steps {
                sh 'echo Hola'
                // sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
                // stash(name: 'compiled-results', includes: 'sources/*.py*') 
            }
        }
    }
}