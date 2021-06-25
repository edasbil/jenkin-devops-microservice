pipeline {
	//agent any
	agent { docker { image 'maven:3-openjdk-11' } }
	stages {
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
				echo "always"
		}
		success {
				echo "success"
		}
		failure {
				echo "failure"
		}
		changed {
				echo "Changed"
		}
	}	
}
