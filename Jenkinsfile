pipeline {
    agent { label 'master' }
    stages {
        stage('git_clone_demo') {
            steps {
                echo 'Hello world!' 
                git credentialsId: '21453014-5ed1-4c30-8ee0-240f8b9f9474', url: 'https://github.com/redprasa/DEMO2.git'
            }
        }
    stage('Build') {
        steps {
            echo 'helloword'
            sh '''
            mvn clean
            mvn compile
            mvn test
            mvn package
            '''
        }
    }
    stage('Unittests') {
        steps {
            echo 'helloword'
        }
    }
    stage('sonar') {
        steps {
            echo 'helloword'
        }
    }
    stage('artifactory') {
        steps {
            echo 'helloword'
        }
    }
    stage('deploy') {
        steps {
            echo 'helloword'
        }
    }
    }
}
