pipeline {
    agent {
        docker {
            image 'shshdxk/maven:3.8.6-jdk-14' 
            args '-v /root/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
