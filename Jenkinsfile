pipeline{
    agent any
    environment{
        JAVA_HOME="C:/Program Files/Java/jdk-21"
        PATH="${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages{
        stage("clone repository"){
            steps{
                git branch: 'main' , url: 'https://github.com/MohammedAteeb/exam.git'
            }
        }
        stage('compile java'){
            steps{
                bat 'javac hello.java'
            }
        }
        stage('run java code'){
            steps{
                bat 'java hello.java'
            }
        }
    }
}
