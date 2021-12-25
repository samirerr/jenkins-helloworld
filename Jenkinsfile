pipeline {
    
     agent { node { label 'agent1' } }
     stages {
         stage('Clone') {
             
             steps {
                script {
                  git 'https://github.com/karimsahebettaba/my-jenkins-file.git'
                }
             }
        }
		
         stage('Build') {
             
             steps {
                script {
                  sh label: '', script: 'javac Main.java'
                }
             }
        }
	
         stage('Run') {
             
             steps {
                script {
                  sh label: '', script: 'java Main'
                }
             }
        }
     }
	}
