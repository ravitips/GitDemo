pipeline{
    agent any
    stages{
        stage('Create file'){
            steps{
                sh 'pwd'
                sh 'rm -rf ravi.txt'
                sh 'touch ravi.txt'
            }
        }
        
        stage('Edit file'){
            steps{
                sh 'echo "Hai Im ravi" > ravi.txt'
            }
        }
        
        stage('Copy file'){
            steps{
                sh 'rm -rf ravi_copy.txt'
                sh 'cp ravi.txt ravi_copy.txt'
            }
        }
        
    }
}
