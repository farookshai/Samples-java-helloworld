pipeline {
    agent any
    stages {
        stage('compile stage'){
            steps{
			withmaven(maven : 'maven_3_5_0'){
			sh 'mvn clean compile'       
        }
    }
    stage('testing stage'){
        steps{
		withmaven(maven : 'maven_3_5_0'){
			sh 'mvn test'
            
            
        }
    }
    
    stage('deployment stage'){
        steps{
            echo 'for testing'
            
        }
    }
    
    stage('deploy'){
        steps{
		withmaven(maven : 'maven_3_5_0'){
			sh 'mvn deploy'
           
        }
    }
    
     }
   }
  }
 }
}
