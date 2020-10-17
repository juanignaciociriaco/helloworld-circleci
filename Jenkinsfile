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
                sh 'apt-get update'
                sh 'apt-get install python3'
                sh 'uname -a'
                sh 'python3 --version'
                // sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
                // stash(name: 'compiled-results', includes: 'sources/*.py*') 
            }
        }
    }
}