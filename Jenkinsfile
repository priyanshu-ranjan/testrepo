pipeline {
         agent any
         stages {
                 stage('Build') {
                 steps {
                     echo 'Hi, this is Priyanshu Ranjan'
                 }
                 }
                 stage('Deploy') {
                 steps {
                    input('Do you want to proceed for testing?')
                 }
                 }
                 stage('Test') {
                 when {
                       not {
                            branch "master"
                       }
                 }
                 steps {
                       echo "Testing Done!"
                 }
                 }
                 stage('Release') {
                 steps {
                    echo('Product release succesful!')
                 }
                 }
                 
              }
}
