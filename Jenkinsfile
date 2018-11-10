pipeline{
agent any
	stages{
		stage('Parallel Stage') {
             		parallel {
                		stage('Build-1') {
                    			agent {
                        		label "RHEL&&TEST"
                    }
                    steps {
                        echo "Running on RHEL&&TEST"
                    }
                }
                stage('Build-2') {
                    agent {
                        label "RHEL&&TEST_1"
                    }
                    steps {
                        echo "Running on RHEL&&TEST_1"
                    }
                }
			}
	}
	}
}
