pipeline {
    agent any
    options {
        skipDefaultCheckout()
    }

    parameters {
        booleanParam(name: 'RUN_PARALLEL', defaultValue: false, description: 'Run parallel stages?')
    }

    stages {
        stage("Parallel Stages") {
            when {
                expression { params.RUN_PARALLEL }
            }
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
}
