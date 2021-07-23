node {
    def mvnHome
    stage('Preparation') { // for display purposes
        // Get some code from a GitHub repository
        git 'https://github.com/irfan-devops/rep1.git'
    }
    stage('mvn clean') {
        // Run the maven build
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
}
       