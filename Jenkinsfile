node {
    echo "start"
    checkout scm

    stage("run") {
    	echo "run"
    	sh "chmod 777 ./hello ""
		sh "./hello"
    }

    echo "end"
}