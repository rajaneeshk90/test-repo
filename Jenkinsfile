
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                checkout scmGit(branches: [[name: '*/draft']], extensions: [], userRemoteConfigs: [[credentialsId: 'gitroot', url: 'https://github.com/rajaneeshk90/test-repo.git']])
                echo 'Hello World'
            }
        }
    }
}



