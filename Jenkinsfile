pipeline {
    agent any
    stages {
        stage("Set Permissions") {
            steps {
                sh "chmod +x gradlew"
            }
        }
        stage("Compile") {
            steps {
                sh "./gradlew compileJava"
            }
        }
        stage("Build") {
            steps {
                sh "./gradlew build"
            }
        }
        stage("Unit test") {
            steps {
                sh "./gradlew test"
            }
        }
    }
}
