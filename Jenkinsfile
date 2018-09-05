pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				dir('D:\software\jenkin\checkout'){
					checkout scm
					echo 'Building the Jenkin Application!'
					stash(name: 'app', includes: 'outputs')
				}	
			}
		}
	}
}