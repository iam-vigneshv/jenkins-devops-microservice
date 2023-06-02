pipeline {

	// agent {docker { image 'maven:3.6.3'}}
	agent any

	environment {
		// mavenHome = tool 'myMaven'
		dockerHome = tool 'myDocker'
		PATH = "$dockerHome/bin:$PATH"
		// PATH = "$mavenHome/bin:$PATH"
	}

		stages{
	
			stage('Build') {

				steps {
				echo 'Docker --version'
				// bat 'mavin --version'
				bat 'docker version'
				echo "Build"
				}
			}
			stage('Test') {
				steps {
					echo "Test"
				}
				
			}

			stage('Integration Test') {
				steps {
					echo "Integration Test"
				}
				
			}
		
		}

		post {
			always {
					echo "I run when u run always"
			}
			success {
				echo "I run when u pass"

			}
			failure{
				echo "I'm in failed stage"

			}
		}
}

