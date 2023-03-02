node() {
   stage('Build'){
	cmd_exec('echo "git -v"')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
