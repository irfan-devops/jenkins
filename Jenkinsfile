pipeline {
    agent any
    tools {
     maven 'maven-3.8.1'
	}
	stages {
	   stage ('gitclone') {
	   steps {
	   git branch: 'main', url: 'https://github.com/irfan-devops/login.git'
	   }
	 }
	 
	   stage ('maven version') {
	     steps {
		  sh 'mvn --version'
		 }
		 }
	
	stage('maven clean') {
       steps {
		sh 'mvn clean'
       }
     }
		
	stage('maven validate') {
       steps {
        sh 'mvn validate'
       }
    }
	
    stage('maven compile') {
        steps {
        sh 'mvn compile'
       }
	   }
	   
   	stage('maven test') {
       steps {
        sh 'mvn test'
       }
       }
    stage('maven package') {
        steps {
        sh 'mvn package'
       }
	   }
	  }
    }
