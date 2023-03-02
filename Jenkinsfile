pipeline {
    	agent any
	def workspace = pwd()
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
				git -v
			   }
		     }
	   }
	}
}
