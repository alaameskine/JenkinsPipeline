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
  }
}
