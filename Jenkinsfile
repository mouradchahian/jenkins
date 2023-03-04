node() {
   stage('Build'){
	deleteDir()
	checkout scm
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra . /O /X /E /H /K")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
