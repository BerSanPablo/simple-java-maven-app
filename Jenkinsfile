pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'C:\\Users\\bersa\\Documents\\apache-maven-3.9.2\\bin\\mvn -B -DskipTests clean package'
            }
        }
        stage('Test') {
            steps {
                bat 'C:\\Users\\bersa\\Documents\\apache-maven-3.9.2\\bin\\mvn test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
    }
}
