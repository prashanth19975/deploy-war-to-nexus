pipeline {
    agent any
    stages {
        stage('git clone') {
            steps {
			   git credentialsId: '7055e685-65e1-4ff3-a369-6085c5f4ca7c', url: 'https://github.com/prashanth19975/prashanth19975.git'
             }
             }
		stage('maven version') {
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
	        stage('maven deploy') {
            steps {	 
			    sh 'mvn deploy'
				}
				}
	}

}	