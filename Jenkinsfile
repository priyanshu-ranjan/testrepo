pipeline {
         agent any
         stages {
                 stage('Build') {
                 steps { echo 'Running build phase...' }
                 }
                 stage('Post-Build') {
                 steps { input('Do you want to proceed for testing?') }
                 }
                 stage('Testing') {
                 when {
                       not { branch "master" }
                 }
                 steps { echo "Testing Done!" }
                 }
                 stage('Deployment') {
                 steps { echo('Product deployment succesful!') }
                 }
              }
}
