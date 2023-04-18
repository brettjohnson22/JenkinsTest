pipeline {

  agent any

  stages {

    stage('Test') {
      steps {
        sh 'echo "Testing application..."'
      }
    }

    stage('Build') {
      steps {
        sh 'echo "Building application..."'
      }
    }

    stage('Docker') {
      steps {
        sh 'echo "Building image and pushing to Docker Hub..."'
      }
    }

    stage('Deploy') {
      when {
        branch 'main'
      }
      steps {
        sh 'echo "Deploying application to EC2 instance..."'
      }
    }

  }
}