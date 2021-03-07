pipeline {
    agent any
    stages {
        stage('Build') {
                steps {
			script{
		docker build -t getting-started .
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
