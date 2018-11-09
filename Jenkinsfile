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
            environment {
                USERNAME = 'Jenkins'
            }
            steps {
                echo 'Testing..'
                // echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                echo "Hi Mr. ${USERNAME}"
                echo "I said Hi Doc. ${USERNAME}"
                echo " hello Jenkins"
                //sh 'printenv'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
