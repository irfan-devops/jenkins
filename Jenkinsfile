pipeline {
    agent any

    tools {
     maven 'maven 3.8.1'
	 }
	 
	stages {
	   stage ('git clone') {
	   steps {
	   git branch: 'main', url: 'https://github.com/irfan-devops/login.git'
	   }
	   }
	 
	stage ('mvn version') {
	     steps {
		  sh 'mvn --version'
		 }
		 }
	
	stage('mvn clean') {
       steps {
		sh 'mvn clean'
       }
     }
		
	stage('mvn validate') {
       steps {
        sh 'mvn validate'
       }
    }
	
    stage('mvn compile') {
        steps {
        sh 'mvn compile'
       }
	   }
	   
   	stage('mvn test') {
       steps {
        sh 'mvn test'
       }
       }
    stage('mvn package') {
        steps {
        sh 'mvn package'
       }
	   }
	}
