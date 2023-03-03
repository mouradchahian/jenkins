node() {
   stage('Build'){
	bat: 'cp -r C:/tmp/test .'
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
