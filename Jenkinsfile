pipline {

    agent any

    stages {

        stages("build") {

            steps {
                echo "building application"
                sh "npm install"
                sh "npm build"
            }
        }

        stage("test") {

            steps {
                echo "testing application"
                sh "npm test"
            }

        }

        stage("build") {

            steps {
                echo "building application"
            }

        }
    }
}

