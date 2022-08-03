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
      parallel {
        stage('Determine dir2') {
          steps {
            pwd(tmp: true)
          }
        }

        stage('Determine dir3') {
          steps {
            pwd(tmp: true)
          }
        }

        stage('Determine dir4') {
          steps {
            pwd(tmp: true)
          }
        }

        stage('Determine dir5') {
          steps {
            pwd(tmp: true)
          }
        }

      }
    }

  }
}
