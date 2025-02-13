@Library('github-api-global-lib') _

pipeline {
    agent any

    stages {
        stage('Example') {
            steps {
                script {
                    // გამოიყენეთ ბიბლიოთეკის ფუნქციები
                    def api = new com.darinpope.github.GitHubAPI()
                    def repos = api.getUserRepositories('darinpope')
                    echo "Repositories: ${repos}"
                }
            }
        }
    }
}
