pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }
  }
  post {
    always {
      emailext body: build.result.toString(),
               subject: 'Build operation result',
               to: 'yoan.sanna@netc.fr'
    }
  }
}
