pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        git(url: 'https://github.com/wakaleo/game-of-life.git', branch: 'master', poll: true)
      }
    }
    stage('package') {
      steps {
        sh 'mvn package'
      }
    }
  }
  environment {
    dev = ''
  }
}