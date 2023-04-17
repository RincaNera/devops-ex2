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
      emailext body: "Build #${currentBuild.number} is ${currentBuild.currentResult}",
               subject: "Build operation #${currentBuild.number} result: ${currentBuild.currentResult}",
               to: 'rinca.nera@netc.fr'
    }
  }
}
