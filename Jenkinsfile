pipeline {
    agent any
    environment {
        DOCKER_REPO="leftshiftit"
    }

    stages {
        stage('Pull Image') {
            steps {
                echo "Pulling Image"
            }
        }
        stage('Deploy Image') {
            when {
                branch 'dev'
            }
            steps {
                echo 'I am deploying to dev'
            }
        }
    }
}
