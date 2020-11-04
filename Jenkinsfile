pipeline {

    agent any

    stages {

        stage("build") {

            steps {
                sh 'docker build . -t example'
            }
        }

        stage("test") {

            steps {
                sh 'docker run example sh -c "go test"'
            }
        }
    }

}