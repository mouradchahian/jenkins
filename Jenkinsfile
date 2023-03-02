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
			   git branch: 'vp-rem', url: 'https://github.com/devopshydclub/vprofile-repo.git'
		     }
	   }
	}
}
