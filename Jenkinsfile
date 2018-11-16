pipeline {
	agent none
	stages {
		stage('Windows-Build'){
			agent {label "Win"}
			steps {
			bat'''
			svn upgrade
			cd build
			scons
			'''
			}
		}
	}
}
