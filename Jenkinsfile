pipeline {
  agent { dockerfile true }
  stages {
    stage('log version info') {
       steps {
        sh 'pwd'
	sh 'ls -ltr'
        sh 'mvn --version'
	sh 'mvn -f src/pom.xml clean install'
	sh 'ls src/target/'
	sh 'java -jar src/target/gs-maven-0.1.0.jar'
      }
    }
  }
}
