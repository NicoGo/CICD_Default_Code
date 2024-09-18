pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'python -m py_compile functions.py main.py'
                stash(name: 'compiled-results', includes: '*.py*')
            }
        }
    }
}