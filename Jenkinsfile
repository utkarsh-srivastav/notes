pipeline {
    agent any
    stages {
	    stage('Build image') { // build and tag docker image
        steps {
            echo 'Starting to build docker image'
	sh """docker build -t app ."""

        }
    }

	    stage('Deploying'){

		steps {
			echo 'Deploying...'
        }
	    }


    }
}
