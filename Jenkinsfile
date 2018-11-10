pipeline {
  agent {label 'RHEL&&TEST'}
      stages {
        stage("test") {
            steps {
                parallel (
                    "Unit Test" : {
                        build("unit-test-job")
                    },
                    "Component Test" : {
                        build("component-test-job")
                    },
                    "Build" : {
                        build("build-job")
                    }
                )
            }
        }
    }
}
