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
     triggers {
        cron('*/5 * * * *')
    
    environment {
        AWS_ACCESS_KEY_ID= credentials('AKIAIY44CGLFXKTIDDBA')
        AWS_SECRET_ACCESS_KEY= credentials('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 ')
        AWS_DEFAULT_REGION='eu-central-1b'    
    }
    stages {
        stage('') {

                steps {
                    
                    } 
            }     
     }
}
