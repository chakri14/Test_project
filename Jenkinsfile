pipeline {
	agents any
		stages {
			parallel {
				stage ('Build-Linux_0'){
                			agent {
		                    		label "RHEL&&TEST"
                			}
	                		steps {
        		        		echo "Build job-1"
                			}
	             		}

				stage ('Build-Linux_1'){
			                agent {
			                       label "RHEL&&TEST_1"
                			}
			                steps {
                    				echo "Build job-2"
                			}
             			}
			}
	}
}
