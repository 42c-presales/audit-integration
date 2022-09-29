pipeline {
    agent any 
    stages {
        stage('Audit OpenAPI files') {
            steps {
                audit repositoryName: "${env.GIT_URL}", branchName: "${env.GIT_BRANCH}", credentialsId: '42ctoken', minScore: 75, platformUrl: 'https://platform.42crunch.com', logLevel: 'DEBUG'
            }
        }
    }
}