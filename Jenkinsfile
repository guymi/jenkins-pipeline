pipeline {
  agent any
  stages {
    stage('Step1') {
      steps {
        parallel(
          "Step1": {
            sh 'echo I am in step one'
            
          },
          "step2": {
            sh 'echo I am in step 2'
            
          }
        )
      }
    }
    stage('Last') {
      steps {
        sleep 10
      }
    }
  }
}