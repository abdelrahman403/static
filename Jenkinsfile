pipeline {
    agent any
    stages {
    	stage('Upload to AWS') {
            steps {
                withAWS(region:'us-east-2', credentials:'aws-static') {
                    // do something
                    s3Upload(bucket:"udacity-devops-proj3", includePathPattern:'**/*');
                }
            }
        }
    }
}
