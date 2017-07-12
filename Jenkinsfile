pipeline {
  agent any
  stages {
    stage('') {
      steps {
        parallel(
          "date": {
            sh 'date'
            
          },
          "id": {
            sh 'id'
            
          }
        )
      }
    }
    stage('echo') {
      steps {
        echo 'message'
      }
    }
  }
}