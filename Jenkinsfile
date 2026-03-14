pipeline{

    agent any

    stages{

        stage{

            steps{
                cleanWs()
            }
        }

        stage('build'){
            agent {

                docker{

                    image 'node:18-alpine'
                }

            }
            steps{
                sh 'npm --version'
            }
        }

    }
}