pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				dir('D:\\software\\jenkin\\checkout'){
					checkout scm
					echo 'Building the Jenkin Application!'
				}	
				bat 'make' 
                archiveArtifacts artifacts: 'D:\\software\\jenkin\\target\\*.jar', fingerprint: true
			}	
		}
	}
}