pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				dir('subDir'){
					checkout scm
					echo 'Building the Jenkin Application!'
					stash(name: 'app', includes: 'outputs')
				}	
			}
		}
	}
}