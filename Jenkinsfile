pipeline {
    agent any
    stages {
	    stage('Build image') { // build and tag docker image
        steps {
            echo 'Starting to build docker image'
            script {
                def dockerfile = 'Dockerfile'
		docker.build("my-image:${env.BUILD_ID}", "-f ${dockerfile} ./dockerfiles")
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
