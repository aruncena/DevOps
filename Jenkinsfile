pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M3"
    }

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/aruncena/DevOps.git'
            }

        }
    }
}
