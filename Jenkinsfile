pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "date": {
            timestamps()
            sh 'date'
            
          },
          "id": {
            echo 'id'
            
          }
        )
      }
    }
    stage('echo') {
      steps {
        echo 'message'
        sleep 1
      }
    }
    stage('mail') {
      steps {
        mail(subject: 'test', body: 'test', to: 'jenkins@jenkins.localdomain')
      }
    }
  }
}