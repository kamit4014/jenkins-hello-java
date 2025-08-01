// build via GitHub webhook
// Re-Triggering build via GitHub webhook
// Re-trigger build for webhook test
//Trigger build via webhook on 1-Aug-2025

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
