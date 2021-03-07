pipeline {
    agent any
    stages {
        stage('Build') {
                steps {
                        docker build -t getting-started .

                }
        }
	    stage('Deploying'){

		steps {
			echo 'Deploying...'
        }
	    }


    }
}
