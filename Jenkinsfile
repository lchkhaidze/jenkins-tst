pipeline {
  agent any
  stages {
    stage('Run Maven Project') {
      parallel {
        stage('Run Maven Project') {
          steps {
            sh 'mvn compile test package'
          }
        }

        stage('Maven Version') {
          steps {
            sh 'mvn --version'
          }
        }

      }
    }

    stage('mvn clean test') {
      steps {
        bat 'mvn clean test'
      }
    }

  }
}