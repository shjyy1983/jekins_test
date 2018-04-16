node {
    echo "start"

    stage('checkout') {
    	checkout scm
    }

    stage("run") {
    	echo "run"
    	sh "chmod 777 ./hello"
    	sh """
    		./hello
    	""" 
    }  

    stage("run job1_pipeline") {
    	build job: 'job1_pipeline', parameters: []
    }

    echo "end"
}