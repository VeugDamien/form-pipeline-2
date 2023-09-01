pipeline{
  agent any
  stages {
    stage('Build') {
      agent{
        label 'linux'
      }
      steps {
        sh "echo 'Compilation from test' > toto.txt"
        archiveArtifacts artifacts: 'toto.txt', fingerprint: true
      }
    }
    stage('Test') {
      
      agent{
        label 'windows'
      }
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
