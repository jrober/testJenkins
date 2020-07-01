pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                cmake {
	            	cmakeInstallation('InSearchPath')
		           //generator('Unix Makefiles')
		            cleanBuild()
		            //sourceDir('src')
		            buildDir('build')
		            args('-DVIDEO=ON')
		            buildToolStep {
		                vars('--target', 'install')
		                useCmake()
		            }
        		}		
            }
        }
    }
}