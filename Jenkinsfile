pipeline {
  agent any
  stages {
    stage('Confirm Deploy to Staging') {
      when {
          branch 'main'
      }
      steps {
        echo 'Deploy to Stage'
      }
    }
    stage('Deploy to Staging') {
      when {
        branch 'main'
      }
      steps {
        unstash 'Buzz Java 8'
        echo 'Complete'
      }
    }
  }
}
