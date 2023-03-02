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
			     start cmd.exe /c echo 'hhh'
    			   /$
		     }
	   }
	}
}
