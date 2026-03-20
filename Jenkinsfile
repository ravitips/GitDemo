pipeline{
    agent { label 'server1' }
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
                    rm -rf prasath
                    mkdir prasath
                    mkdir ravi
                """
            }
        }
    }
}
