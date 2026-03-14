pipeline{

    agent any

    stages{

        stage('build'){
            agent {

                docker{

                    image 'node:18-alpine'
                    reuseNode true
                }


            }
            steps{
                sh '''
                        ls -la
                        node --version
                        npm --version
                        npm install --cache .npm
                        npm run build
                        ls -la
                '''
            }
        }

    }
}