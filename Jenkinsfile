node {

    stage('Gitclone') {
	
	    git branch: 'main', credentialsId: '1dfe6426-03e0-443e-a4b6-fd9bbc5d34d5', url: 'https://github.com/Nawazarifa/project.git'
    }
	stage('java version') {
	
	       sh 'java -version'
    }
	stage('maven version') {
	
	      sh 'mvn --version'
	}
	stage('maven validate ') {
	
	      sh  'mvn validate'
	}
	stage ('maven compile') {
	
	      sh  'mvn compile'
    }
	stage('maven test')  {
	
	      sh 'mvn test'
	}
	stage('maven package') {
	
	      sh 'mvn package'
	}
	stage('maven deploy') {
	
	      sh 'mvn deploy'
	}
}
		  
		  
