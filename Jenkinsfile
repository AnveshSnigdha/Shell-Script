pipeline {
    agent any
    stages {
        stage('CLONING CODE FROM GITHUB') {
            steps {
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/AnveshSnigdha/Shell-Script']]])
            echo "clone the code from github"
            }
        }
        stage('BUILDING THE CODE') {
            steps {
                echo "Building the code by Maven"
            }
        }       
        stage('TESTING THE CODE') {
            steps {
                echo "Testing the code by running Unit Test Cases"
            }
        }
        stage('DEPLOYING THE APPLICATION ON SERVERS') {
            steps {
                echo "Deployment in Test Levels"
            }
        } 
        stage('RELEASE ON TO PRODUCTION SERVERS') {
            steps {
                echo "Deployment on PROD SERVERS"
            }
        }
        stage('POST-BUILD NOTIFICATION TO DEV TEAM') {
            steps {
                echo "Trigger mail to AnveshSteam@gmail.com"
            }
        }
    }    
}
