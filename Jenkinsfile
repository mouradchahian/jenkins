node() {
   stage('Build'){
	deleteDir()
	checkout scm
	sh "git clone git@github.com:D4UDigitalPlatform/mymarque-aws-infra.git /tmp/${BUILD_ID}"
	sh "cp -r  /tmp/${BUILD_ID}/config/aws/_init ."
	sh "cp -r /tmp/${BUILD_ID}/deployment/scripts ."
	sh "rm -rf /tmp/${BUILD_ID}"
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
