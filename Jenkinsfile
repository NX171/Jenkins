pipeline {
    agent any
    options {
        skipDefaultCheckout()
    }

    stages {
        stage("Building") {
            steps {
                input message: 'Proceed with build?'

                script {
                    // This is a comment
                    echo "Building"
                }
            }
        }
    }
}
