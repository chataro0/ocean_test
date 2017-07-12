pipeline {
  agent any
  stages {
    stage('switch') {
      steps {
        catchError() {
          sh '"exit 1"'
        }
        
      }
    }
    stage('if') {
      steps {
        parallel(
          "OK": {
            echo 'OK'
            
          },
          "NG": {
            echo 'NG'
            
          }
        )
      }
    }
  }
}