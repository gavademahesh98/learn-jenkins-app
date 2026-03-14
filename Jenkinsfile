pipeline{

    agent any

    stages{

        stage('preclean'){

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