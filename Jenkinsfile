pipeline{
    agent {
        label 'java-maven'
    }

    options { 
		buildDiscarder(logRotator(numToKeepStr: '10')) 
	} 
	
	tools {
		jdk 'JAVA_8'
	}
	
	stage('build and unit test'){
		steps {			
            sh "./gradlew clean assemble"
		}
	}

}
