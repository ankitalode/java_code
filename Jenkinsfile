pipeline {
  agent { dockerfile true }
  stages {
    stage('log version info') {
       steps {
        sh 'pwd'
	sh 'ls -ltr'
        sh 'mvn --version'
	sh 'cd /var/lib/jenkins/workspace'
	sh 'ls -ltr'
      }
    }
  }
}
