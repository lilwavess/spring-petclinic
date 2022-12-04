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
        sh 'mvn sonar:sonar -Dsonar.login=bffa84635c364a1693d3f1036e743a29'
      }
    }

  }
}