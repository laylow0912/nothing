pipeline {
    agent { any 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
	stage('test'){
	    steps {
		echo 'execute test'
	    }
	}
	stage('deploy'){
	    steps {
		echo 'execute deploy'
	    }
	}
    }
}
