pipeline {
    	agent any
	tools {
        	git "Default"
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
			   bat "C:\Users\mchahian\AppData\Local\Programs\Git\cmd\git.exe"
		     }
	   }
	}
}
