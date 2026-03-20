pipeline {
    agent { label 'server1' }

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
