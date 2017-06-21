#!groovy
@Library('Bluemix') _
pipeline {
    agent any
    stages {
        stage("Parse") {
            steps {
                AddProductToManifest("some-ui32","1.2.0")
            }
        }
    }
}
