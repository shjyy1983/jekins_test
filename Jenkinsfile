pipeline {
    agent any 
    stages {
        stage('Checkout') { 
            steps {
                checkout scm
            }
        }
        stage('Run') { 
            steps {
	            sh "chmod 777 ./hello"
		    	sh """
		    		./hello
		    	"""
		    	build job: 'job2_pipeline', parameters: []
            }
        }
    }
}