pipeline {
  agent any
  stages {
    stage('pull from git') {
      steps {
        sh 'git \'https://github.com/akshitdeep/auto_dep\''
      }
    }

    stage('compile') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('package') {
      steps {
        sh 'mvn package'
      }
    }

  }
}