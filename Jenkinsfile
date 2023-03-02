pipeline {
    	agent any
	tools {
        	git "gitbin"
    	}
	stages {
	    stage('Build'){
		steps{
		    checkout scm
		    echo "mourad"
		}
	     }
	     stage('EnvInitialization') {
		     steps{
			   bat "echo 'hello'"
		     }
	   }
	}
}
