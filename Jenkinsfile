pipeline{
    agent any
    Environment {
        DOCKER_USERNAME = credentials('shamanth123')
        DOCKER_PASSWORD = credentials('Mlore@1434')
        Tag=buildNumber()
    }
    stages{
        stage ('Checkout'){
            steps{
                git 'https://github.com/shamanthnb-cmd/may-1.git'
            }
            }
        }
        stage('Docker Build and Push'){
            steps{
                docker login registry.hub.docker.com -u $DOCKER_USERNAME -p $DOCKER_PASSWORD
                docker build -t shamanth123/may-1:$Tag .
                docker push shamanth123/may-1:$Tag
            }
        }
    }
}