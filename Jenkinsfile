pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        git(url: 'https://github.com/woody0927/guava-tips', branch: 'master')
      }
    }
    stage('Build') {
      steps {
        pwd(tmp: true)
      }
    }
  }
}