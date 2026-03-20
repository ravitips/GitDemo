pipeline {
    agent any

    stages {
        stage('Basic Commands') {
            steps {
                sh """
                    ls
                    pwd
                    whoami
                """
            }
        }

        stage('Create Directory') {
            steps {
                sh """
                    rm -rf ravi
                    mkdir ravi
                """
            }
        }
    }
}
