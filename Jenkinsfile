node() {
   stage('Build'){
        deleteDir()
	checkout scm
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\config\\aws . /O /X /E /H /K")
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\deployment . /O /X /E /H /K")
	cmd_exec("docker-compose -f _init\\docker\\docker-compose_dev.yml build")
	cmd_exec("docker-compose -f _init\\docker\\docker-compose_dev.yml up -d")
	cmd_exec("docker-compose -f _init\\docker\\docker-compose_build.yml ps")
	cmd_exec('docker exec app_mym_back bash -c "bash ./var/www/tmp/scripts/install.sh"')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
