pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/kamit4014/jenkins-hello-java.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the Java project...'
                bat 'javac Hello.java' // Change to your actual Java file
            }
        }

        stage('Run') {
            steps {
                echo 'Running the Java program...'
                bat 'java Hello' // Change to your actual class name
            }
        }
    }
}
