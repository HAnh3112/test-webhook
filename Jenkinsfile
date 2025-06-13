pipeline {
 agent any
 
 stages {
	stage('clone'){
		steps {
			echo 'Cloning source code'
			git branch:'main', url: 'https://github.com/HAnh3112/test-webhook.git'
		}
	}
    stage('build') {
		steps {
			echo 'build project'
		}
	}
    stage('tests') {
            steps{
                echo 'running test...'
            }
        }
 }

}//end pipeline
