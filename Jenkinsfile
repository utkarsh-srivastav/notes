pipeline {
    agent any
    stages {
	    stage('Build image') { // build and tag docker image
        steps {
            echo 'Starting to build docker image'
		script {

			docker.build('app', 'docker/app')
		}
        }
    }

	    stage('Deploying'){

		steps {
			echo 'Deploying...'
        }
	    }


    }
}
