// Triggering build via GitHub webhook
pipeline {
    agent any

    stages {
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
