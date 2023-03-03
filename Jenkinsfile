node() {
   stage('Build'){
	#cmd_exec('git clone https://github.com/mouradchahian/test2.git /tmp/test')
	bat: 'cp -r C:/tmp/test .'
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
