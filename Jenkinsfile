pipeline{
    agent any

    tools {
       // stage('checkout'){
            // steps{
                // checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github access', url: 'https://github.com/sreenivas449/java-hello-world-with-maven.git']]])
            // }
        // }
        stage('checkout'){
            checkout 'scm'
        }
        stage('build'){
            steps{
               sh 'mvn package'
               sh 'mvn clean install'
            }
       }
    }
}