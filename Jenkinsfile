pipeline {
    	agent any
	stages {
	    stage('Build'){
		steps{
		    checkout scm
		    echo "mourad"
		    script {
			workspace = pwd()
			echo workspace
			git -v
		   }
		}
	     }
	}
}
