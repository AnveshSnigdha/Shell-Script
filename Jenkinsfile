 pipeline {
    agent any
    stages {
        stage ("cloning code from github"){
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/anvesh']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/AnveshSnigdha/Shell-Script.git']]])
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
                echo "deployment in test levels L1,l2,L3 and L4"
            }
        }
        stage ("release the code on servers"){
            steps {
                echo "deployment on production Productioenv@gmail.com"
            }
        }
        
    }
}

