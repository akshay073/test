pipeline {
  agent any
  stages {
    stage('pull from git') {
      steps {
        git 'https://github.com/akshay073/test'
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