node() {
   stage('Build'){
	deleteDir()
	checkout scm
	cmd_exec("xcopy C:/Users/mchahian/Desktop/mymarque-aws-infra/config/aws/_init ./ /y")
	cmd_exec("xcopy C:/Users/mchahian/Desktop/mymarque-aws-infra/deployment/scripts ./ /y")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
