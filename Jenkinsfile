pipeline{
    agent any
    stages{
        stage('details'){
            steps{
                sh """
                    pwd
                    ls
                    whoami
                    hostname
                """
            }
        }
        stage('Create Directory'){
            steps{
                sh """
                    rm -rf ravi
                    mkdir ravi
                """
            }
        }
    }
}
