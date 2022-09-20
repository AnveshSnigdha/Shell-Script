
 pipeline {
    agent any
    stages {
        stage ("cloning code from github"){
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/AnveshSnigdha/Shell-Script.git']]])
                echo "cloning code from github" 
            }
        }
        stage ("BUILD THE CODE"){
            steps {
                echo "building the code by maven"
            }
        }
        stage ("test the code"){
            steps {
                echo "testing the code by running the different test cases"
            }
        }
        stage ("deploying the code on server"){
            steps {
                echo "deployment in test levels"
            }
        }
        stage ("release the code on servers"){
            steps {
                echo "deployment on production servers@gmail.com"
            }
        }
        
    }
}

