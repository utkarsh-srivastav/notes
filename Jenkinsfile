pipeline {
    agent any
    stages {
	    stage('Build') { // build and tag docker image
		steps {
		    	script {  
				sh "docker build -t utkarsh233.jfrog.io/techm-uttu/hello:1.0.${env.BUILD_ID} ."
		    	}
		}
	    }

	    stage('Upload'){
		steps {
			script {  
				docker.withRegistry('https://crepantherx.jfrog.io', 'jfrog') {
					sh "docker push utkarsh233.jfrog.io/techm-uttu/hello:1.0.${env.BUILD_ID}"
				}
			}
		}
	    }
    }
}
