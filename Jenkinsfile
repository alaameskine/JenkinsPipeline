pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat(script: 'echo "Building"', returnStatus: true, returnStdout: true)
      }
    }

    stage('Test') {
      steps {
        bat(script: 'echo "Testing"', returnStatus: true, returnStdout: true)
      }
    }

    stage('Deploy') {
      steps {
        bat(script: 'echo "Deploying"', returnStatus: true, returnStdout: true)
      }
    }

    stage('Determine dir') {
      steps {
        pwd(tmp: true)
      }
    }

    stage('Catching errors') {
      steps {
        load 'C:\\Groovy\\New Pipeline\\Jenkins-Pipelines'
        error 'There is no groovy file!'
      }
    }
    post {
      always {
          junit 'build/reports/**/*.xml'
      }
    }
  }
}
