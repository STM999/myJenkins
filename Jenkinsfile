 node('docker') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        bat 'dotnet build'

    stage 'Docker Build'
        bat 'docker build -t myjenkins myJenkins/.'

    stage 'Deploy'
        bat 'docker run -d -p 80:80 --name myjenkins myjenkins'
}