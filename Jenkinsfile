pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'ubuntu:20.04' 
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