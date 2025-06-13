pipeline {
 agent any
 
 stages {
	stage('clone'){
		steps {
			echo 'Cloning source code'
			git branch:'main', url: 'https://github.com/huudqtmu/projectnet.git'
		}
	} // end clone
 // end stages
    stage ('build') {
		steps {
			echo 'build project netcore'
			bat 'dotnet build  --configuration Release'
		}
	}
    stage ('tests') {
            steps{
                echo 'running test...'
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
 }

}//end pipeline
