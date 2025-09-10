pipeline {
    agent any;
    stages {
        stage("Build") {
            steps {
                echo "Building with Maven"
            }
        }
        stage("Testing") {
            steps {
                echo "Running automatic unit and integration tests with JUnit."
            }
        }
        stage("Analysis") {
            steps {
                echo "Using SonarQube for static code analysis, including static application security testing (SAST)."
            }
        }
        stage("Security Scan") {
            steps {
                echo "Using Synk for open-source dependency zero day scanning and suggestions for improvements."
            }
        }
        stage("Deploy to staging") {
            steps {
                echo "Deploying to a Amazon Web Services EC2 server."
            }
        }
        stage("Integration tests on staging") {
            steps {
                echo "Running integration tests on the EC2 staging server. Testing API correctness using Postman."
            }
        }
        stage("Deploying to production") {
            steps {
                echo "Pushing to the AWS EC2 prod server."
            }
        }
    }
}