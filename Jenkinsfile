#! groovy

pipeline {
  agent any
  stages {
    stage('Setup') {
      steps {
        echo "Setup"
        
        sh "bundle config set --local path 'vendor/bundle'"
        sh "bundle check || bundle install --jobs=4 --retry=3"
      }
    }
    stage('Build') {
      steps {
        echo "Building"
        sh "bundle exec fastlane build"
      }
    }
  }
}
