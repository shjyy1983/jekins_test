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
    
    echo "end"
}