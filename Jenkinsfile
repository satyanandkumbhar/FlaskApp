pipeline {
  agent any
  stages {
    stage ("Build") {
      steps {
        sh 'pip3 install -r requirements.txt'
      }
    }
    stage ("Build Docker Image") {      
      steps {
        sh 'docker build -t flaskapp .'
      }
    }
    stage ("Deploy") {
      steps {
        sh 'docker run -p 5000:5000 flaskapp'
      }
    }
  }
}
