pipeline {

	// agent {docker { image 'maven:3.6.3'}}
	agent any

	// environment {
	// 	mavenHome = tool 'myMaven'
	// 	// dockerHome = tool 'myDocker'
	// 	// PATH = "$mavenHome/bin:$dockerHome/bin:$PATH"
	// 	PATH = "$mavenHome/bin:$PATH"
	// }

		stages{
	
			stage('Build') {

				steps {
				// sh 'mavin --version'
				// sh 'docker version'
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

