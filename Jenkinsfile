node() {
   def directory = pwd();
   stage('Build'){
	deleteDir()
	checkout scm
	cmd_exec('git clone https://github.com/devopshydclub/vprofile-project.git /tmp/test')
	cmd_exec('Xcopy /E /I /tmp/test/. /var/build')
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
