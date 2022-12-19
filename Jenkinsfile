pipline {

    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000' 
        }
    }
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

