pipeline {
    	agent any
	tools { git 'C:\Program Files\Git\cmd\git.exe' }
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
