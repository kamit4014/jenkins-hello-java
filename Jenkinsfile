pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Starting pipeline for jenkins-hello-java...'
            }
        }

        stage('Build') {
            steps {
                echo 'Listing .java files in repo:'
                bat 'dir /s *.java'

                echo 'Compiling Java files:'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java program:'
                bat 'java HelloWorld'
            }
        }
    }
}
