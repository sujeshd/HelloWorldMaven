pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
                withMaven(maven : 'Apache_Maven_3.6.0'){
                        bat "mvn clean compile"
                }
            }
        }
        stage('Test'){
            steps {
                withMaven(maven : 'Apache_Maven_3.6.0'){
                        bat "mvn test"
                }

            }
        }
        stage('Deploy') {
            steps {
               withMaven(maven : 'Apache_Maven_3.6.0'){
                        bat "mvn deploy"
                }

            }
        }
    }
}
