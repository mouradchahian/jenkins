node() {
   stage('Build'){
	cmd_exec('git clone https://github.com/devopshydclub/vprofile-project.git /tmp/test')
	cmd_exec('cp -r /tmp/test .')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
