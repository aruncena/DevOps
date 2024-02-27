pipeline{
    agent any
    stages{
        stage('SCMCheckout'){
            steps{
                git branch: '${BRANCH}', url: 'https://github.com/aruncena/DevOps.git'
            }
        }
        stage('QA_Deploy'){
            steps{
                echo "Deploting to QA"
            }
        }
    }
}
