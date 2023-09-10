//See https://www.jenkins.io/doc/book/pipeline/syntax/ for explanation of `when { changeset .. }`

pipeline {
    agent any
    stages {
        stage('Test Suite 1') {
            when {
                changeset 'test/suite1/**'
            }
            steps {
                sh "echo run test suite 1"
            }
        }
        stage('Test Suite 2') {
            when {
                changeset 'test/suite2/**'
            }
            steps {
                sh "echo run test suite 2"
            }
        }
    }
}
