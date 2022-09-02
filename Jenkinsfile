pipeline {
	agent any
	stages {
		stage('compile') {
			steps {
					echo "Compiled Successfully!!";
			}
		
		}
	
		stage('Junit') {
			steps {
					echo "Junit passed Successfully!!";
			}
		
		}
	
		stage('Quality') {
			steps {
					echo "Quality passed Successfully!!";
					/*sh exit ("1");*/
			}
		
		}
		
		stage('Deploy') {
			steps {
					echo "Deployed Successfully!!";
			}
		
		}
	
	}

	post {
		always {
			echo "This will always run"
		}
		success {
			echo "This will run only if successfull"
		}
		failure {
			echo "This will run only if failed"
		}
		unstable {
			echo "This will run only if the run was marked as unstable"
		}
		changed {
			echo "This will run only if the state of the pipeline is changed"
			echo "For Example: if the pipeline was previously failing but now successfull"
		}
	
	}
}
