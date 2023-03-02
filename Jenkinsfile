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
			   script { folderName = new java.text.SimpleDateFormat("yyyyMMddHHmmssMs").format(new Date()); }
			   sh "git clone git@github.com:D4UDigitalPlatform/mymarque-aws-infra.git /tmp/${folderName}"
			   sh "cp -r  /tmp/${folderName}/config/aws/_init ."
			   sh "cp -r /tmp/${folderName}/deployment/scripts ."
			   sh "rm -rf /tmp/${folderName}"
		     }
	   }
	}
}
