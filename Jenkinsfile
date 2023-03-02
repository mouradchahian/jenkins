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
			   bat script: $/
			     'C:\Program Files\Git\cmd\git.exe' {} \;
    			   /$
		     }
	   }
	}
}
