pipeline {
  agent any
  stages {
    stage('Run Maven Project') {
      parallel {
        stage('Run Maven Project') {
          steps {
            sh 'mvn clean test'
          }
        }

        stage('Maven Version') {
          steps {
            sh '''mvn --version
git --version
java -version'''
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