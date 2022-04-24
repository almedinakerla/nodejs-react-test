pipeline {
  agent any
  tools {nodejs "node"}
  stages {
    stage('Build') {
      steps {
        git 'https://github.com/almedinakerla/nodejs-react-test'
        bat 'npm install'
      }}}


}
