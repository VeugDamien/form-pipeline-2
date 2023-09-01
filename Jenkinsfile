pipeline{
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Compilation from test"
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
