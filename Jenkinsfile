pipeline {
  agent { dockerfile true }
  stages {
    stage('log version info') {
       steps {
        sh 'pwd'
	sh 'ls -ltr'
        sh 'mvn --version'
	sh 'cd src'
	sh 'ls -ltr'
	sh 'mvn clean install'
	sh 'java -jar target/gs-maven-0.1.0.jar'
      }
    }
  }
}
