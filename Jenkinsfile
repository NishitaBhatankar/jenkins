pipeline {
         agent any
         stages {
                 stage('One') {
                 steps {
                     echo 'Hi'
                 }
                 }
                 stage('Two') {
                 steps {
                    input('Proceed?')
                 }
                 }
                 stage('Three') {
                 when {
                       not {
                            branch "master"
                       }
                 }
                 steps {
                       echo "Hello world"
                 }
                 }
                 
              }
}
