 node('node') {
    stage 'Checkout'
        checkout scm

    stage 'Build'
        sh 'docker build -t myjenkins .'
}