 node('node') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        sh ' dotnet build'
}