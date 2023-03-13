pipeline {
    agent any

    stages {
        stage('build') {
            tools {
                gradle 'gradle'
                jdk 'jdk8'
            }
            steps {
                sh 'gradle clean'
                sh 'gradle -x test build'
            }
        }
    }
}
