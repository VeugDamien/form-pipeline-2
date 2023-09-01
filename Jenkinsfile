pipeline{
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Compilation from test"
        sh "make"
      }
    }
    stage('Test') {
        steps {
            echo 'Testing..'
        }
    }
    stage('Deploy') {
        steps {
            echo 'Deploying....'
        }
    }
  }
}
