pipeline{
    agent any
    Environment{
        Java_Home="C:/Program Files/Java/jdk-21"
        Path="${Java_Home}\\bin;${env.Path}"
    }
    Stages{
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
