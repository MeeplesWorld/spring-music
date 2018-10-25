pipeline{
    agent {
        label 'java-maven'
    }

    options { 
		buildDiscarder(logRotator(numToKeepStr: '10')) 
	} 
	
    stages {
	
        stage('build and unit test'){
            steps {			
                sh "./gradlew clean assemble"
            }
        }
    }
}
