pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh """
                    sudo cp -r index.html /var/www/html/index.nginx-debian.html
                """
            }
        }
        stage('Deploy'){
            steps{
                sh """
                    sudo systemctl restart nginx
                """
            }
        }
    }
}
