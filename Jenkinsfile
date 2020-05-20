pipeline {
     agent { label 'REDHAT'}
	 triggers { pollSCM('* * * * *') }
	 stages {
	     stage('clone & compile') {
		    steps {
               git branch: 'declerative'
               url: 'https://github.com/seshi7/game-of-life.git'
               sh 'mvn compile'			   
			}
		 }
	 
	 }
	 

}
