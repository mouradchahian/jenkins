node() {
   stage('Build'){
	cmd_exec('echo "Buils starting..."')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
