#!/usr/bin/env Groovy

pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh './mvnw -V -B clean package'
                sh 'java -cp target dev.troublemaker.App'
            }
        }
    }
}