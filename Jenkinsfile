node() {
   stage('Build'){
	deleteDir()
	checkout scm
	cmd_exec("xcopy /y /tmp /")
	cmd_exec("xcopy /y /tmp /")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
