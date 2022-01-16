#!/usr/bin/env Groovy

pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh './mvnw -V -B clean package'
                sh 'java -cp target/java-hello-world-1.0.SNAPSHOT.jar dev.troublemaker.App'
            }
        }
    }
}