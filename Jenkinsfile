 node('docker') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        sh 'dotnet build'

    stage 'Docker Build'
        sh 'docker build -t myjenkins myJenkins/.'

    stage 'Deploy'
        sh 'docker run -d -p 80:80 --name myjenkins myjenkins'
}