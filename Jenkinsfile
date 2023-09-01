pipeline{
  agent any
  stages {
    stage('Build') {
      steps {
        echo "Compilation from test" > toto.txt
        archiveArtifacts artifacts: 'toto.txt', fingerprint: true
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
