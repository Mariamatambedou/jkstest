pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                // Clone the Git repository
                bat 'git clone https://github.com/Mariamatambedou/jkstest.git'
            }
        }

        stage('Build') {
            steps {
                // Compile your Java code with the full path to Main.java
                bat 'javac jkstest/Main.java'
            }
        }

        stage('Run') {
            steps {
                // Run your Java program
                bat 'java -cp jkstest Main'
            }
        }
    }
}
