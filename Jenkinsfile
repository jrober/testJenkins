pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                	bat 'mkdir build'
                	bat 'cd build'
                	bat 'cmake ..'
                	bat 'cmake --build .'
        		}		
            }
        }
    }
