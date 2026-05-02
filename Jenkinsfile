pipeline{
    agent any
    stages{
        stage ('Checkout'){
            steps{
                git 'https://github.com/shamanthnb-cmd/may-1.git'
            }
        }
        stage('Build'){
            steps{
                echo 'Building...'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing...'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying...'
            }
        }
    }
}