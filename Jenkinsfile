pipeline {
    agent any

    stages {

        stage('Checkout Git Content') {
            steps {
                dir('git-content') {
                    git branch: 'develop',
                        url: 'https://github.com/Dineshgcoder/Jenkins-Git-Assignment.git'
                }
            }
        }

        stage('Verify Files') {
            steps {
                sh 'ls -la git-content'
            }
        }
    }
}
