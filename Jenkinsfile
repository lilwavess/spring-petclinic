pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        sh 'mvn clean install'
      }
    }
    stage('Stage 2') {
      steps {
        sh 'mvn sonar:sonar -Dsonar.login=myAuthenticationToken'
      }
    }
  }
}
