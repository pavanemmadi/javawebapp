pipeline {
    agent any 
    stages {
        stage('Clean') { 
            steps {
                'mvn clean' 
            }
        }
        stage('Validate') { 
            steps {
                'mvn validate' 
            }
        }
        stage('Compile') { 
            steps {
                'mvn Compile'  
            }
        }
        stage('Test') { 
            steps {
                'mvn test -DskipTests'  
            }
        }
        stage('Package') { 
            steps {
                'mvn package -DskipTests'  
            }
        }
         stage('Verify') { 
            steps {
                'mvn verify -DskipTests'  
            }
        }
         stage('Install') { 
            steps {
                'mvn install -DskipTests'   
            }
        }
    }
}
