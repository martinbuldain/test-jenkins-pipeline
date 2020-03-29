pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo git diff --dirstat=files,0 HEAD~1 | sed 's/^[ 0-9.]\+% //g'
                echo 'Printing output'
            }
        }
    }
}