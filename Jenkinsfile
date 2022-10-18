pipeline {
    agent { any 'maven:3.3.3' }
    stages {
        stage('build') {
	    environment {
        	DISABLE_AUTH = 'true'
        	DB_ENGINE    = 'sqlite'
    	}

            steps {
                sh 'mvn --version'
		sh 'printenv'
            }
        }
	stage('test'){
	    steps {
		echo 'execute test'
		sh 'printenv'
	    }
	}
	stage('deploy'){
	    steps {
		echo 'execute deploy'
	    }
	}
    }
     post {
        always {
            junit 'build/reports/**/*.xml'
        }
    }
}
