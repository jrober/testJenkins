pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
            		def test = "1"
            		cmakeBuild buildDir: 'build', 
            		cmakeArgs: '-DVIDEO=ON -DTEST=ON',
            		buildType: 'Release', 
            		cleanBuild: true, 
            		//generator: 'Ninja', 
            		installation: 'InSearchPath', 
            		//sourceDir: '${env.WORKSPACE}', 
            		steps: [[envVars: '''A=B
						C=D''', 
						withCmake: true,
						args: '']]
        		}		
            }
        }
    }
