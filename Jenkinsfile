pipeline {
	agent any
	tools {
	    maven "MAVEN3"
	    jdk "OracleJDK8"
	}

	stages {
	    stage('Fetch code') {
            steps {
               git branch: 'vp-rem', url: 'https://github.com/devopshydclub/vprofile-repo.git'
            }

	    }

	    stage('Build'){
	        steps{
	           
	        }

	        post {
	           success {
	              echo 'Now Archiving it...'
	           }
	        }
	    }

	    stage('UNIT TEST') {
            steps{
                
            }
        }
	}
}