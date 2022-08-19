
pipeline {
    agent any
    tools {
        jdk 'jdk'
        maven 'maven'
       
    }
    stages {
        stage("build project") {
            
            steps {
                script{
                    echo "Starting Deploy for environment "
            }
              // git 'https://github.com/mhkarimi/spring-boot-security-oauth2-jwt-example.git'
                echo "Java VERSION"
                sh 'java -version'
                echo "Maven VERSION"
                sh 'mvn -version'
                echo 'building project...'
                sh "mvn compile"
                sh "mvn package"
                //sh "mvn test"
                sh "mvn clean install"
            }
        }
    }
}
