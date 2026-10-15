pipeline{
	agent any
	tools{
		nodejs 'nodejs2400'
	}
	stages{
		stage("Basic Setup"){
			steps{
				sh '''
				apt update -y
				apt upgrade -y
				apt install sudo vim -y
				'''
			}
		}
		stage("Hello"){
			steps{
	
				sh "node -v"
			}
		}
	}
	post{
		always{
			sh 'echo This is always execute';
			//deleteDir()
		}
	}

}
