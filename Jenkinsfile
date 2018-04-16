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

    stage("run job2_1") {
    	build job: 'job2_1', parameters: []
    }

    echo "end"
}