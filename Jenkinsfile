pipeline{
    agent any

    tools {
         maven 'maven3.8.1'
         jdk 'java'
    }

        stage('build'){
            steps{
               sh 'mvn package'
               sh 'mvn clean install'
            }
        }
}