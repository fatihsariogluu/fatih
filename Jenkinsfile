#!/usr/bin/env groovy

pipeline {
   agent {
    label 'master'
    }
    options {
        timestamps()
        retry(1)
        buildDiscarder(logRotator(numToKeepStr: '5'))
        timeout(time: 45, unit: 'SECONDS')
        //skipDefaultCheckout()
        disableConcurrentBuilds()
    }
    stages {
        stage('Run Docker') {

                steps {
                      docker run docker-hello-world:latest
                    } 
            }     
     }
}
