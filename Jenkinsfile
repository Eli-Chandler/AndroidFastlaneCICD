pipeline {
    agent { label 'fastlane' }
    stages {
        stage('Install bundle') {
            steps {
                bat 'bundle config path vendor/bundle'
                bat 'bundle install'
            }
        }
        stage('Run fastlane') {
            steps {
                bat 'bundle exec fastlane distribute'
            }
        }

    }
}
