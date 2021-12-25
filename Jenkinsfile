pipeline {
    
     node("agent1")
     stages {
         stage('Clone') {
             agent any
             steps {
                script {
                  git 'https://github.com/karimsahebettaba/my-jenkins-file.git'
                }
             }
        }
		
         stage('Build') {
             agent any
             steps {
                script {
                  sh label: '', script: 'javac Main.java'
                }
             }
        }
	
         stage('Run') {
             agent any
             steps {
                script {
                  sh label: '', script: 'java Main'
                }
             }
        }
     }
	}
