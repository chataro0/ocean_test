pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "date": {
            sh 'echo "date"'
            
          },
          "id": {
            sh 'echo "id"'
            
          }
        )
      }
    }
    stage('echo') {
      steps {
        echo 'message'
      }
    }
    stage('mail') {
      steps {
        mail(subject: 'test', body: 'test', to: 'jenkins@jenkins.localdomain')
      }
    }
  }
}