pipline {

    agent any

    stages {

        stages("build") {

            steps {
                echo "building application"
                sh "npm install"
                sh "npm run build"
            }
        }

        stage("test") {

            steps {
                echo "testing application"
                sh "npm run test"
            }

        }

        stage("deploy") {

            steps {
                echo "deploying application"
            }

        }
    }
}

