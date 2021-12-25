node {
  stage('Clone') {
    git 'https://github.com/karimsahebettaba/my-jenkins-file.git'
  }
  stage('Build') {
    sh label: '', script: 'javac Main.java'
  }
  stage('Run') {
    sh label: '', script: 'java Main'
  }
}
