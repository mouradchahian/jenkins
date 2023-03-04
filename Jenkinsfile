node() {
   stage('Build'){
	checkout scm
	cmd_exec('git clone https://github.com/D4UDigitalPlatform/mymarque-aws-infra.git')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
