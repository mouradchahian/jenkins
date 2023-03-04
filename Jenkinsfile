node() {
   stage('Build'){
	deleteDir()
	checkout scm
	cmd_exec("copy -r  C:/Users/mchahian/Desktop/mymarque-aws-infra/config/aws/_init .")
	cmd_exec("copy -r C:/Users/mchahian/Desktop/mymarque-aws-infra/deployment/scripts .")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
