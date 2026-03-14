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
                    reuseNode true
                }

            }
            steps{
                sh 'npm --version'
            }
        }

    }
}