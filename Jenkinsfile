pipeline {
  agent any
  stages {
    stage('initialize') {
      parallel {
        stage('initialize') {
          steps {
            bat 'mvn --version'
          }
        }

        stage('Print') {
          steps {
            echo 'this is it'
          }
        }

      }
    }

    stage('Install') {
      steps {
        bat 'mvn clean install'
      }
    }

    stage('Test') {
      steps {
        bat 'mvn test'
      }
    }

  }
}