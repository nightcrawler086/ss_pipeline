pipeline {
	agent { label 'jenkins-slave' }
	stages {
		stage ('Build') {
			steps {
				// Define steps here
				checkout([$class: 'GitSCM', branches: [[name: '*/develop']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '211038fb-4f4b-453a-b615-7c04a5455f89', url: 'http://git.local.lab/root/ss.git']]])
			}
		}
		stage ('Infra') {
			steps {
				// Define steps here
				echo "Hello from Infra Stage"
			}
		}
		stage ('Test') {
			steps {
				// Define steps here
				echo "Hello from Test Stage"
			}
		}
	}
}
