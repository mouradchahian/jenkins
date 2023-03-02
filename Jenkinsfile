pipeline {
    	agent any
	stages {
	    stage('Build'){
		steps{
		    checkout scm
		    echo "mourad"
		}
	     }
	     stage('EnvInitialization') {
		     steps{
			   sh "git clone git@github.com:D4UDigitalPlatform/mymarque-aws-infra.git ."
		     }
	   }
	}
}
