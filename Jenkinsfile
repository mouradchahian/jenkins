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
		     tools { gitH 'git2' }
		     steps{
			   script {
				workspace = pwd()
				echo workspace
				gitH -v
			   }
		     }
	   }
	}
}
