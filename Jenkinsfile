pipeline {
    agent any

    stages {
        stage('Git URL') {
            steps {
                echo 'Hello World'
                git branch: 'main', url: 'https://github.com/tarshyak/pub1.git'
                
            }
        }
        
        stage('Build'){
            
            steps{
              
             bat ''' javac Trash.java  
             java Trash'''
            }
        }
        
        stage('BatFile Stage'){
            steps{
                bat 'Trash1.bat'
            }
        }
        
        
        
    }
    
    post{
        success{
            echo "Everything executed correctly"
        }
    }
}
