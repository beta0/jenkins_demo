pipeline{
    agent any
    
    tools{
        maven 'mvn-3.8.1'
    }
    stages{
        stage('Build'){
            steps{
                sh "mvn clean package spring-boot:repackage"
                sh "printenv" // 将环境变量打印到console中
            }
        }
    }
}