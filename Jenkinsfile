pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
            		cmakeBuild buildDir: '${build_dir}', buildType: '${config}', cleanBuild: true, generator: 'Ninja', installation: 'InSearchPath', sourceDir: '${env.WORKSPACE}', steps: [[envVars: '''A=B
						C=D''', withCmake: true]]
        		}		
            }
        }
    }
