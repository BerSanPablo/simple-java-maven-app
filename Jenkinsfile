pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'mvn.cmd -B -DskipTests clean package'
            }
        }
    }
}
