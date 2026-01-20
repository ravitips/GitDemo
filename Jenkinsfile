pipeline{
    agent any
    stages{
        stage('find my identity'){
            steps{
                sh """
                    whoami
                """
            }
        }
         stage('find my workspace'){
            steps{
                sh """
                    pwd
                """
            }
        }
        stage('build and deploy'){
            steps{
                sh """
                    echo 'This is my pipeline page - version 1' > /var/www/html/index.nginx-debian.html
                    sudo systemctl restart nginx
                """
            }
        }
    }
}
