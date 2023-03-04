node() {
   stage('Build'){
	deleteDir()
	checkout scm
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\config\\aws . /O /X /E /H /K")
	bat("xcopy C:\\Users\\mchahian\\Desktop\\mymarque-aws-infra\\deployment . /O /X /E /H /K")
	cmd_exec("docker-compose -f _init\\docker\\docker-compose_build.yml --build --no-cache")
	bat "docker-compose -f _init\\docker\\docker-compose_build.yml logs"
	bat "docker exec -it app-${BUILD_ID} bash"
	bat "mkdir -p \\var\\build"
	bat("xcopy \\var\\www\\tmp \\var\\build /O /X /E /H /K")
	bat("cd \\var\\build")
	bat("composer -v")
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
