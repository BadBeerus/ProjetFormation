#!/usr/bin/env groovy

pipeline {
    agent any

try {
		stages {
			stage('Build') {
				steps {
					echo 'Building ${env.BUILD_ID}'
				}
			}
			stage('Test') {
				steps {
					echo 'Testing ${env.BUILD_ID}'
				}
			}
			stage('Deploy') {
				steps {
					echo 'Deploying ${env.BUILD_ID}'
				}
			}
		}
	}
catch (exc) {
		echo "Une erreur s'est produite, le build ne sera pas release"
	}
}