pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
            		bat 'rmdir build'
                	bat 'mkdir build'
                	bat 'cd build'
                	bat 'cmake ..'
                	bat 'cmake --build .'
        		}		
            }
        }
    }
