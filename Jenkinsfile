pipeline{
    agent any
    
    parameters{
        string(name: 'VERSION_NUMBER', defaultValue: '1', description: 'Version Number for your app')
        string(name: 'NGINX_HTML_FILE', defaultValue: '/var/www/html/index.nginx-debian.html', description: 'Nginx index html file path')
        choice(name: 'SERVICE', choices: ['nginx', 'apache', 'flask'], description: 'type of service')
    }
    
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
                    echo 'This is my pipeline page - version ${params.VERSION_NUMBER}' > ${params.NGINX_HTML_FILE}
                    sudo systemctl restart ${params.SERVICE}
                """
            }
        }
    }
}
