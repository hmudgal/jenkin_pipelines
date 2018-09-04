pipeline{
	agent none
	stages{
		stage('Build'){
			agent {
				node{
					label 'builder'
				}
			}
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