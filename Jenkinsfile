node() {
   stage('Build'){
	deleteDir()
	checkout scm
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\config\\aws . /O /X /E /H /K")
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\deployment . /O /X /E /H /K")
	bat "docker-compose CONTAINER_NAME=${BUILD_ID} --project-name=${BUILD_ID} --file ./_init/docker/docker-compose_aws.yml build --no-cache"
        bat "docker-compose CONTAINER_NAME=${BUILD_ID} --project-name=${BUILD_ID} --file ./_init/docker/docker-compose_aws.yml up -d"
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
