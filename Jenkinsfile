pipeline {
  agent any
  stages {
    stage('Git') {
      steps {
        echo 'Start'
        git(url: 'https://github.com/BoondockRiley/Postgres', branch: 'main', credentialsId: 'github-token2')
      }
    }

    stage('Test') {
      steps {
        echo 'End'
      }
    }

  }
}