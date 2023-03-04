node() {
   stage('Build'){
	deleteDir()
	checkout scm
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\config\\aws . /O /X /E /H /K")
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\deployment . /O /X /E /H /K")
	bat "docker-compose -f .//_init//docker//docker-compose_dev.yml up -d --build"
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
