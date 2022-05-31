pipeline {
  agent any
  stages {
    stage('Build buzz') {
      steps {
        sh 'echo "Hello World"'
        sh '''
                    echo "Multiline shell steps works for first stage"
                    ls -lah
                '''
      }
    }

    stage('Test buzz') {
      steps {
        sh 'echo "Hello from test"'
        sh '''
                    echo "Multiline shell steps works for second stage"
                    ls -lah
                '''
      }
    }

  }
}