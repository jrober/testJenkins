pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
            		cmakeBuild buildDir: 'build', 
            		buildType: 'Release', 
            		cleanBuild: true, 
            		//generator: 'Ninja', 
            		installation: 'InSearchPath', 
            		//sourceDir: '${env.WORKSPACE}', 
            		steps: [[envVars: '''A=B
						C=D''', 
						withCmake: true,
						args: '-DVIDEO=ON -DTEST=ON']]
        		}		
            }
        }
    }
