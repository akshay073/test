pipeline {
  agent any
  stages {
    stage('pull from git') {
      steps {
        bat 'git \'https://github.com/akshitdeep/auto_dep\''
      }
    }

    stage('compile') {
      steps {
        bat 'mvn compile'
      }
    }

    stage('package') {
      steps {
        bat 'mvn package'
      }
    }

  }
}