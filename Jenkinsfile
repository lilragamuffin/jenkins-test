pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh './gradle check'
      }
    }
  }
  post {
    always {
      junit 'build/reports/**/*.xml'
    }
  }
}
