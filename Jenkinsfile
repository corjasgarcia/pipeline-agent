/*

Test agents in a pipeline
testing...
*/
pipeline {
	agent (label 'master')
	/*
	tools{
	docker 'docker'
	}
	*/
    stages {
        stage('Example Build') {
			
			/*agent {
				
				}
            */
            steps {
			   sh 'docker ps'
               echo 'Hello, Maven'
               // sh 'mvn --version'
            }
        }
        stage('Example Test') {
			agent ('master')
            /*agent {
                docker { image 'node:7-alpine' }
            }
			*/
            steps {
                echo 'Hello, JDK'
                //sh 'java -version'
            }
        }
    }
}