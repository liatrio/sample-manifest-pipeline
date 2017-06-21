#!groovy
@Library('Bluemix') _
pipeline {
    agent any
    parameters {
        string(name: "Product")
        string(name: "Version")
    }
    stages {
        stage("Parse") {
            steps {
                AddProductToManifest("some-ui32","1.2.0")
            }
        }
    }
}
