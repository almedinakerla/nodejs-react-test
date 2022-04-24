pipeline {
  agent any
  tools {nodejs "node"}
  environment {
    CI = 'true'
 }
  stages {
    stage('Build') {
      steps {
        git 'https://github.com/almedinakerla/nodejs-react-test'
        sh 'npm install'
      }}}


}
