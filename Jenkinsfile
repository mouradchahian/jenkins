node() {
   stage('Build'){
	deleteDir()
	checkout scm
	script: '''#!/bin/bash
                 COPY "C:\Users\mchahian\Desktop\mymarque-aws-infra" . 
         '''
   }
}
def cmd_exec(command) {
    return bat(returnStdout: true, script: "${command}").trim()
}
