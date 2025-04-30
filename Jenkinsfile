pipeline{
    agent any
    tools{
        'jdk21'
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
