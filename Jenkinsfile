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
	stage('sonar scan'){
	
	sh 'mvn sonar:sonar \
        -Dsonar.host.url=http://13.214.159.208:9000 \
        -Dsonar.login=8a3c12dfcb8d66ba723efea4bced920a23b99c40'
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
		  
		  
