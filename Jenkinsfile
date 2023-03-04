node() {
   stage('Build'){
	deleteDir()
	checkout scm
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\config\\aws . /O /X /E /H /K")
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\deployment . /O /X /E /H /K")
	bat "CONTAINER_NAME=${BUILD_ID} C:\\Program Files\\Docker\\Docker\\resources\\bin\\docker-compose --project-name=${BUILD_ID} --file _init/docker/docker-compose_aws.yml build --no-cache"
        bat "CONTAINER_NAME=${BUILD_ID} C:\\Program Files\\Docker\\Docker\\resources\\bin\\docker-compose --project-name=${BUILD_ID} --file _init/docker/docker-compose_aws.yml up -d"
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
