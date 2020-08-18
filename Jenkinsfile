pipeline {
  agent any
  stages {
    stage('pull from git') {
      steps {
        git(url: 'https://github.com/akshay073/test', branch: 'brother')
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