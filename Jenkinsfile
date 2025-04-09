pipeline {
    agent any
    options {
        skipDefaultCheckout()
    }

    stages {
        parallel {
            stage("Building") {
                steps {
                    script {
                        // This is a comment
                        echo "Building"
                    }
                }
            }
            stage("Testing") {
                steps {
                    script {
                        // This is a comment
                        echo "Testing"
                    }
                }
            }
        }
    }
}
