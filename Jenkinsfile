pipeline {
  agent {label 'RHEL&&TEST'}
    stages {
        parallel{
          stage ('Build-1'){
             steps {
                echo 'Build-1'
              }
            }
          stage ('Build-2'){
            steps {
              echo 'Build-2'
            }
          }
      }
    }
}
