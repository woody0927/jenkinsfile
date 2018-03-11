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
        sh '''echo ${PATH}
echo ${M2_HOME}
echo ${MAVEN_HOME}
mvn clean install'''
        pwd(tmp: true)
      }
    }
  }
}