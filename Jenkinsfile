pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('pullcode') {
      steps {
        git(url: 'https://github.com/suryavamshi123/jenkinswar.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'mvn clean package'
      }
    }
  }
}