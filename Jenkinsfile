pipeline{
 agent { label 'java-runtime' }
    tools {
         maven 'maven3.8.1'
         jdk 'java'
    }

    stages{
       // stage('checkout'){
            // steps{
                // checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github access', url: 'https://github.com/sreenivas449/java-hello-world-with-maven.git']]])
            // }
        // }
        stage('code from git'){
            steps{
                git 'git@github.com:manikanta4448/sms.git'
            }
            
        }
        stage('build'){
            steps{
                echo "build steps in main branch"
               sh 'mvn package'
               sh 'mvn clean install'
            }
       }
    }
}
