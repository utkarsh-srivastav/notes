pipeline {
    agent any
    stages {
	    stage('Build image') { // build and tag docker image
        steps {
            echo 'Starting to build docker image'
		script {  
			docker.withRegistry('https://registry.example.com', 'jfrog') {
        			def customImage = "docker build -t crepantherx.jfrog.io/techmahindra-docker-dev-local/todo:${env.BUILD_ID} ."
       				/* Push the container to the custom Registry */
        			customImage.push()
    			}

		}
        }
    }

	    stage('Deploying'){

		steps {
			echo 'Deploy'
        }
	    }


    }
}
