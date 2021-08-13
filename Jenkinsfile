pipeline {
    agent any    
 	stages {
	   stage ('Git clone') {
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
	stage('sonarscan') {
       steps {
        sh 'mvn sonar:sonar -Dsonar.host.url=http://34.122.106.232:9000 -Dsonar.login=3d0b5f204f34d66e11eaf7f7d6c9d96e0eea271d'
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
