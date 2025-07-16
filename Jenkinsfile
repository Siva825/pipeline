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
                git clone 'https://github.com/devopswithcloud/spring-petclinic.git'
                sh 'mvn validate'
            }
        }
    }
}
