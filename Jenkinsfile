node() {
   stage('Build'){
	deleteDir()
	checkout scm
	cmd_exec("COPY 'C:\Users\mchahian\Desktop\mymarque-aws-infra' .")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
