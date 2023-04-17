pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        mail (subject: 'Build operation result', body: 'test', to: 'yoan.sanna@netc.fr')
      }
    }
  }
}
