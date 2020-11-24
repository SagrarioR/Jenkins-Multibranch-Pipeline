 pipeline {
        agent any
        stages {
                stage('First') {
                        steps {
                                script {
                                        echo "Building 1"
                                        env.EXECUTE = 'true'
                                }
                        }
                }

 

                stage('Second') {
                        when {
                                expression {
                                        env.EXECUTE == 'true'
                                }
                        }

 

                        steps {
                                script {
                                        echo "Updating second stage"
                                        echo "${env.EXECUTE}"
                                }
                        }
                }

 

                stage('Third') {
                        when {
                                expression {
                                        env.EXECUTE == 'false'
                                }
                        }
                        steps {
                                script {
                                        echo "Deploying yes"
                                }
                        }

 

                }
        }
} 
