node {
    echo "start"
    checkout scm

    stage("run") {
    	echo "run"
    	chmod 777 ./hello 
		./hello
    }

    echo "end"
}