/*

Test agents in a pipeline
testing...
*/
pipeline {
	agent any
	
    stages {
        stage('Example Build') {
		
            
            steps {
			DOCKER_HOME = tool "docker"
                echo 'Hello, Maven'
               // sh 'mvn --version'
            }
        }
        stage('Example Test') {
             
            steps {
                echo 'Hello, JDK'
                //sh 'java -version'
            }
        }
    }
}