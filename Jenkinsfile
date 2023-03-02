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
			   sh "git clone git@github.com:D4UDigitalPlatform/mymarque-aws-infra.git /tmp/${folderName}"
			   sh "cp -r  /tmp/${folderName}/config/aws/_init ."
			   sh "cp -r /tmp/${folderName}/deployment/scripts ."
			   sh "rm -rf /tmp/${folderName}"
		     }
	   }
	}
}
