node() {
	environment {

    		PATH = "C:\\WINDOWS\\SYSTEM32"

	}
	stage('Build'){
		    checkout scm
		    bat(returnStdout: true, script: "echo 'hello'").trim()
	}
}
