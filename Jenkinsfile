pipeline {
    agent {
        docker { image 'node:7-alpine' }
    }
    stage('Initialize')
    {
        def dockerHome = tool 'MyDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
