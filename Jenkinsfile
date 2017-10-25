/*

Test agents in a pipeline
testing...
*/
pipeline {
	agent any
	tools{
	docker 'docker'
	}
    stages {
        stage('Example Build') {
		
            
            steps {
			   sh 'docker ps'
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