node() {
   stage('Build'){
	cmd_exec('echo "git clone git@github.com:D4UDigitalPlatform/mymarque-aws-infra.git"')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
