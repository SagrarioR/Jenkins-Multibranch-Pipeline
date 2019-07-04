pipeline {
        agent any 
        stages {
                stage('First') {
                        steps {
                                sh 'echo "Building"'
                        }
                }

 

                stage('Second') {
                        steps {
                                sh 'echo "Updating second stage"'
                        }
                }

 

                stage('Third') {
                        steps {
                                sh 'echo "Deploying"'
                        }

 

                }
        }
}
