pipeline{
	agent any
	tools{
		nodejs 'nodejs2400'
	}
	stages{
		stage("Hello"){
			steps{
	
				sh "node -v"
			}
		}
	}
	post{
		always{
			sh 'echo This is always execute';
			deleteDir()
		}
	}

}
