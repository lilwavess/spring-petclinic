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
        sh 'mvn sonar:sonar -Dsonar.login=sqa_6f75eec612717d3f4b37f525f7bd37aaab1911b0'
      }
    }

    stage('Stage 3') {
      steps {
        sh 'ansible-playbook -i hosts stage3.yml'
      }
    }

  }
}