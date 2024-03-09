 node('node') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        bat 'dotnet build'

    stage 'Ls'
        bat 'ls'

    stage 'Docker Build'
        bat 'docker build -t myjenkins .'
}