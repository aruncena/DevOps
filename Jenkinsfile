pipeline{
    agent {
        label 'ec2'
    }
    stages{
        stage('SCMCheckout'){
            steps{
                git branch: '${BRANCH}', url: 'https://github.com/aruncena/DevOps.git'
            }
        }
        stage('QA_Deploy'){
            steps{
                sh " scp -o StrictHostKeyChecking=no index.html root@3.109.132.1:/var/www/html/"
            }
        }
    }
}
