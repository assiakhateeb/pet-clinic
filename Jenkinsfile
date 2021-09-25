pipeline {
    agent 'slave' 
    stages {
        stage('Clone GitHub Repositry') {
            steps {
                git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic' 
            }
        }
    }
}
