pipeline {
    agent any
       stages {
        stage('Checkout') {
            steps {
                sh 'git clone https://github.com/Sudhamshetty7/Terraform_jenkin.git'
		sh 'chmod 777 docker.sh'    
			}
		}	
        stage('Terraform Init') {
            steps {
                script {
                    sh 'terraform init'
                }
            }
        }       
        stage('Terraform Apply') {
            steps {
                script {
                    sh 'terraform apply --auto-approve'
                }
            }
        }    
    }
}
