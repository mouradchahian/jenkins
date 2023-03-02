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
			   script {
				workspace = pwd()
				echo workspace
				git -v
			   }
		     }
	   }
	}
}
