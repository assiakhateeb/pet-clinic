pipeline {
    agent { label 'slave' }
    stages {
        stage('Clone GitHub Repositry') {
            steps {
                git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic' 
            }
        }
	stage('Change current directory') { 
	    steps {
	    	dir('spring-petclinic') {
                   // some block
                }
	    }
	}
    }
}
