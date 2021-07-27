node {
    stage('Preparation') { // for display purposes
        // Get some code from a GitHub repository
      git branch: 'main', url: 'https://github.com/irfan-devops/login.git'
    }
    stage('mvn clean') {
        // Run the maven build
		sh 'mvn clean'
       }
        
	stage('mvn validate') {
        // Run the maven build
        sh 'mvn validate'
       }

    stage('mvn compile') {
        // Run the maven build
        sh 'mvn compile'
       }
   	stage('mvn test') {
        // Run the maven build
        sh 'mvn test'
       }
       
    stage('mvn package') {
        // Run the maven build
        sh 'mvn package'
       }
	stage('mvn deploy') {
        // Run the maven build
        sh 'mvn deploy'
       }
}
       
	   
