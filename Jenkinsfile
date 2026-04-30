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
        echo 'Deploying the Application'
      }
    }

  }
}