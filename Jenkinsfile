pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                sh 'mkdir build'
                sh 'cd build'
                sh 'cmake ..'
                sh 'cmake --build .' 
            }
        }
    }
}