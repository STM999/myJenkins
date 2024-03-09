 node('node') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        bat 'dotnet build'

    stage 'Docker Build'
        bat 'docker build -t myjenkins .'
}