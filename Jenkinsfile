pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'echo \'Building it\''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'echo \'Testing it!!!\''
          }
        }

        stage('API_test') {
          steps {
            echo 'echo \'API Testing!!!\''
          }
        }

      }
    }

    stage('Archiving') {
      steps {
        echo 'echo \'Archiving\''
      }
    }

  }
}