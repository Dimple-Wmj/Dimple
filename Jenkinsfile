// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
   
    stages {
        stage('Build') {    //stage('Build')
            steps {
                echo 'Building..'
                sh 'echo "Hello Jenkins > test.txt'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                //只有后一个字符串支持美元符号的字符串插值
                username = 'Jenkins'
                echo "Hello Mr.${username}"
                echo "I said, Hello Mr.${username}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
