 pipeline{
    agent {
        label 'java-slave'
    }
    tools{
        maven 'Maven 3.8.9'
    }
     
    stages{
        stage('build'){
            steps{
                echo "hi this is siva"
                sh 'rm -rf spring-petclinic'
                sh 'git clone https://github.com/devopswithcloud/spring-petclinic.git'
                dir('spring-petclinic'){
                  sh 'mvn validate'  
                }
                
                }
            }
    }
}
