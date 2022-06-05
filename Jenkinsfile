pipeline {
  agent any
  stages {
    stage('Confirm Deploy to Staging') {
      when {
          branch 'main'
      }
      steps {
        input(message: 'Deploy to Stage', ok: 'Yes, let\'s do it!')
      }
    }
    stage('Deploy to Staging') {
      when {
        branch 'main'
      }
      steps {
        unstash 'Buzz Java 8'
        sh 'Complete'
      }
    }
  }
}
