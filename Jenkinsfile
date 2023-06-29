// Create pipeline with agent maven and with a stage build that print the maven version
pipeline {
    agent {
        docker {
            image 'maven:3.6.3-openjdk-11'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
```