#! groovy

pipeline {
  agent any
  stages {
    stage('Setup') {
      steps {
        echo "Setup"
        
        echo "Starting..."
      }
    }
    stage('Build') {
      steps {
        echo "Building"
        sh "fastlane android build"
      }
    }
  }
}
