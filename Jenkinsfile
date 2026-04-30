pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building the Java core application.'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing the Java Applicaton.'
          }
        }

      }
    }

    stage('Deployment') {
      steps {
        input(message: 'Do you want to realy deploy', id: 'ok')
        echo 'Deploying the Application'
      }
    }

  }
}