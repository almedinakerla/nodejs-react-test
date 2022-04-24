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
      }}
    stage('Test') {
      steps {
        sh './jenkins/scripts/test.sh'
            }
       }
    stage('Deliver') {
      steps {
        sh './jenkins/scripts/deliver.sh'
        input message: 'Finished using the web site? (Click "Proceed" to continue)'
        sh './jenkins/scripts/kill.sh'
      }
    }


	
  }


}
