#!groovy
@Library('Bluemix') _
pipeline {
    agent any
    parameters {
        string(name: "Product", description: "Name of the product to be added to the manifest")
        string(name: "Version", description: "Version of the product to be added or updated")
    }
    stages {
        stage("Parse") {
            steps {
                AddProductToManifest("some-ui32","1.2.0")
            }
        }
    }
}
