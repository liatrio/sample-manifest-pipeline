#!groovy
@Library('Bluemix') _
pipeline {
    agent any
    stages {
        stage("Parse") {
            steps {
                AddProductToManifest()
            }
        }
    }
}
