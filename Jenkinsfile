pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/amalbouabid/JobTest.git"
            }
        }
        stage('build') { 
            steps {
                sh "cd JobTest/JobTest/src/  && javac HelloWorld.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd JobTest/JobTest/src/  && java HelloWorld"
            }
        }
    }
}

