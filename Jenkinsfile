pipeline {
  agent any
  stages {
    stage('Loop') {
      steps {
        script {
          allModules.each(){
            echo it }
          }

        }
      }

    }
    environment {
      module1 = '1'
      module2 = '2'
      module3 = '3'
      module4 = '4'
    }
  }