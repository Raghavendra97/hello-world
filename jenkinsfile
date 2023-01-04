pipeline {
    agent any
    environment {
        PATH="/opt/apache-maven-3.8.7/bin:4PATH"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('SCM') {
            steps {
                git 'https://github.com/Raghavendra97/hello-world.git'
            }
        }
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
 
