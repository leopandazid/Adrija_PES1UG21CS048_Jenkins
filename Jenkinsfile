pipeline {
  agent any
  
  stages{
    stage('Build') {
      steps {
        script {
          sh 'g++ -o executable main/PE1UG21CS048.cpp'
        }
        echo 'Build stage successful'
      }
    }

    stage('Test') {
      steps {
        script {
          sh './executable'
        }
        echo 'Test Successful'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment Successful'
      }
    }
  }

  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}

      
