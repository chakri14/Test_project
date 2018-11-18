pipeline {
	agent any
	stages {
        stage('Parallel Stage') {
            parallel {
				stage('Build'){
					agent { label "RHEL" }
					steps {
					bat'''
					svn upgrade
					cd build
					scons
					'''
					}
					post {
						always {
							archiveArtifacts artifacts: 'build/Bin/,software/tests/TestData/ImageService/', fingerprint: true
						}
					}
				}
 			}
		}
	}
}
