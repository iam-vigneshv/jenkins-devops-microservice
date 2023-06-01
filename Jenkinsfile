pipeline {

	agent any

		stages{
	
			stage('Build') {

				steps {

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
			sucess {
				echo "I run when u pass"

			}
			failure{
				echo "I'm in failed stage"

			}
		}
}

