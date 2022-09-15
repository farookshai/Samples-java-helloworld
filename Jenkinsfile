pipeline {
    agent any
    tools{
        maven 'mvn'
        jdk 'jdk'
    }
    stages {
        stage('code'){
            steps{
                echo'coding'
        }
    }
    stage('build'){
        steps{
            echo'building'
            sh 'mvn clean'
            sh 'mvn install 3.8.6'
        }
    }
    
    stage('test'){
        steps{
            echo 'for testing'
            sh 'mvn test'
            sh 'mvn install 3.8.6'
        }
    }
    
    stage('deploy'){
        steps{
            echo'deploying'
        }
    }
    
}
}
