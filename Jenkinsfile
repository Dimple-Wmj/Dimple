// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
   
    stages {
        stage('Build') {    //stage('Build')
            steps {
                echo 'Building..'
                sh 'touch text.txt && echo "Hello Jenkins" > test.txt'
            }
        }
        stage('Test') {
            steps {
                environment {
                    username = 'Jenkins'
                }
                echo 'Testing..'
                // echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                echo "Hi Mr.${username}"
                echo "I said Hi Mr.${username}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
