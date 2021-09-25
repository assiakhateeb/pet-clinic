pipeline {
    agent { label 'slave' }
    stages {
        stage('Clone GitHub Repositry') {
            steps {
	        // Git step. It performs a clone from the petClinic repository. 
                git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic' 
            }
        }
	stage('Change current directory') { 
	    steps {
	        // cd spring-petclinic
	    	dir('spring-petclinic') {
                   // some block
                }
	    }
	}
	stage('Last Stage') {
	    steps {
	    // ./mvnw package
	        script{
		    "./mvnw package"
		}
	    }
	}
    }
}
