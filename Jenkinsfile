#!groovy
@Library('Bluemix') _
pipeline {
    agent any
    parameters {
        string(name: "Product", description: "Name of the product to be added to the manifest")
        string(name: "Version", description: "Version of the product to be added or updated")
    }
    stages {
        stage("Update Manifest") {
            steps {
                AddProductToManifest( params.Product, params.Version )
            }
        }
        stage("Deploy manifest") {
            steps{
                input 'Ready to deploy manifest'
                DeployAllProducts('manifest.yml')
            }
        }
    }
}
