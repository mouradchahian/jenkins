node() {
   stage('Build'){
	deleteDir()
	checkout scm
	cmd_exec("git clone git@github.com:D4UDigitalPlatform/mymarque-aws-infra.git /tmp/${BUILD_ID}")
	cmd_exec("cp -r  /tmp/${BUILD_ID}/config/aws/_init .")
	cmd_exec("cp -r /tmp/${BUILD_ID}/deployment/scripts .")
	cmd_exec("rm -rf /tmp/${BUILD_ID}")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
