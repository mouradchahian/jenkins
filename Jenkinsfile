node() {
   stage('Build'){
	bat: 'git clone https://github.com/mouradchahian/jenkins.git'
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
