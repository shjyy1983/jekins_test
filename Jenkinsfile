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
		    	build job: 'job1_1', parameters: []
            }
        }
    }
}