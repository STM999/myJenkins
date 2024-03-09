 pipeline {
     agent any
     stages {
         stage('Example') {
             steps {
                 echo 'Hello World'
             }
         }
     }
 }

 node('docker') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        sh "docker build -t myjenkins ."
}