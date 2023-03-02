pipeline {
    	agent any
	tools { git 'git' }
	stages {
	    stage('Build'){
		steps{
		    checkout scm
		    echo "mourad"
		}
	     }
	     tools { git 'git' }
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
