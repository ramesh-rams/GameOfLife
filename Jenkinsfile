pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        git(url: 'https://github.com/wakaleo/game-of-life.git', branch: 'master', poll: true)
      }
    }
  }
  environment {
    dev = ''
  }
}