pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script {
                    sh "git diff --dirstat=files,0 HEAD~1 | sed ==~ s/^[ 0-9.]\+% //g"
                    echo 'Printing output'
                }
            }   
        }
    }
}