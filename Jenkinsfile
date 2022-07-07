pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'echo "Building"'
      }
    }

    stage('Test') {
      steps {
        bat 'echo "Testing"'
      }
    }

    stage('Deploy') {
      steps {
        bat 'echo "Deploying"'
      }
    }

    stage('Change directory') {
      steps {
        dir(path: 'https://github.com/alaameskine/flexbox') {
          sh 'echo "Hello flexbox"'
        }

      }
    }

  }
}