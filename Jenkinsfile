pipeline {
    agent {
        label "RHEL&&TEST"
    }
    agent any
    stages {
        stage ('Build'){
            agent {
                label "RHEL&&TEST"
            }
            steps {
                echo "Build job"
            }
        }
    }
}
 
