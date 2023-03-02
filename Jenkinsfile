node() {
   stage('Build'){
	cmd_exec('git clone https://github.com/devopshydclub/vprofile-project.git /temp/test')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
