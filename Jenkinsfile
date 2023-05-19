//DECLARATIVE

pipeline {
	agent any
	//agent { docker { image 'maven:3.6.3'}}
	// agent { docker { image 'node:13.8'}}
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				// sh 'node --version'
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "env.BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"
				echo "JOB_NAME - $env.JOB_NAME"
	}
		}
		stage('test') {
			steps {
				echo "test"
			}
		}
		stage('Integration test') {
			steps {
				echo "Integration test"
			}
		}

	} 
	post {
		always {
			echo 'I am awesome. I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
}