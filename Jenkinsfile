pipeline{
    agent {label "master"}
    stages {
        stage("checkout"){
           steps {
            git branch: "main", url: "https://github.com/ganeshm06/SpringPetClinic.git"
           }
        }
        stage("build"){
            steps {
                sh "mvn compile"
            }
        }   
        stage("Test"){
            steps{
                sh 'mvn test'
            }
        }
        
    }
}
