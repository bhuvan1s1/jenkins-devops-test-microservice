/*
//Scripted coding : old model
node {
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
	stage('SIT') {
		echo "SIT"
	}
	stage('NFT') {
		echo "NFT"
	}
} */

//declarative scripting - new

pipeline {
	//agent any
	agent {
    docker {
        image 'maven:3.6.3'
    }
}
	stages{
		stage('Development'){
			steps {
				echo "Development"
			}
		}
		stage('Functional Testing'){
			steps {
				echo "Functional Testing"
			}
		}
		stage('SIT Testing'){
			steps {
				echo "SIT Testing"
			}
		}
		stage('NFT Testing'){
			steps {
				echo "NFT Testing"
			}
		}
	}
	post {
		always {
			echo " Gets executed always"
		}
		success {
			echo "Success execution"
		}
		failure {
			echo "Failure execution"
		}
	}
}
