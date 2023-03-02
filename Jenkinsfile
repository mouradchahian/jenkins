node() {
	environment {

    		PATH = "C:\\WINDOWS\\SYSTEM32"

	}
	stage('Build'){
		    checkout scm
		    cmd_exec('echo "Buils starting..."')
	}
	def cmd_exec(command) {
	    return bat(returnStdout: true, script: "${command}").trim()
	}
}
