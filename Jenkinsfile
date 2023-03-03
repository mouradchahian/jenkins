node() {
   stage('Build'){
	bat: 'git -v'
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
