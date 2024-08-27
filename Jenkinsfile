pipeline {
    agent any

    stages {
        stage('Git-CheckOut') {
            steps {
                git branch: 'main', url: 'https://github.com/jaiswaladi246/10-Tier-MicroService-Appliction.git'
            }
        }
        
        stage('Docker Image Build Addservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/adservice') {
                    
                    sh 'docker build -t raghava017/adservice:latest .'
                    sh 'docker push raghava017/adservice:latest'
                    sh 'docker rmi raghava017/adservice:latest'
						}
					}
                }
            }
        }
        
        stage('Docker Image Build cartService') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/cartservice/src') {
                    
                    sh 'docker build -t raghava017/cartservice:latest .'
                    sh 'docker push raghava017/cartservice:latest'
                    sh 'docker rmi raghava017/cartservice:latest'
						}
					}
                }
            }
        }
		
		stage('Docker Image Build checkoutservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/checkoutservice') {
                    
                    sh 'docker build -t raghava017/checkoutservice:latest .'
                    sh 'docker push raghava017/checkoutservice:latest'
                    sh 'docker rmi raghava017/checkoutservice:latest'
						}
					}
                }
            }
        }
        
        
		stage('Docker Image Build currencyservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/currencyservice') {
                    
                    sh 'docker build -t raghava017/currencyservice:latest .'
                    sh 'docker push raghava017/currencyservice:latest'
                    sh 'docker rmi raghava017/currencyservice:latest'
						}
					}
                }
            }
        }
        
        
        stage('Docker Image Build emailservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/emailservice') {
                    
                    sh 'docker build -t raghava017/emailservice:latest .'
                    sh 'docker push raghava017/emailservice:latest'
                    sh 'docker rmi raghava017/emailservice:latest'
						}
					}
                }
            }
        }
        
		stage('Docker Image Build frontend') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/frontend') {
                    
                    sh 'docker build -t raghava017/frontend:latest .'
                    sh 'docker push raghava017/frontend:latest'
                    sh 'docker rmi raghava017/frontend:latest'
						}
					}
                }
            }
        }
        
        
		stage('Docker Image Build loadgenerator') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/loadgenerator') {
                    
                    sh 'docker build -t raghava017/loadgenerator:latest .'
                    sh 'docker push raghava017/loadgenerator:latest'
                    sh 'docker rmi raghava017/loadgenerator:latest'
						}
					}
                }
            }
        }
		
		stage('Docker Image Build paymentservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/paymentservice') {
                    
                    sh 'docker build -t raghava017/paymentservice:latest .'
                    sh 'docker push raghava017/paymentservice:latest'
                    sh 'docker rmi raghava017/paymentservice:latest'
						}
					}
                }
            }
        }
        
		stage('Docker Image Build productcatalogservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/productcatalogservice') {
                    
                    sh 'docker build -t raghava017/productcatalogservice:latest .'
                    sh 'docker push raghava017/productcatalogservice:latest'
                    sh 'docker rmi raghava017/productcatalogservice:latest'
						}
					}
                }
            }
        }
        
		stage('Docker Image Build recommendationservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/recommendationservice') {
                    
                    sh 'docker build -t raghava017/recommendationservice:latest .'
                    sh 'docker push raghava017/recommendationservice:latest'
                    sh 'docker rmi raghava017/recommendationservice:latest'
						}
					}
                }
            }
        }
        
		stage('Docker Image Build shippingservice') {
            steps {
                script{
                    withDockerRegistry(credentialsId: 'DockerHub-Cred', toolName: 'Dokcer-Repository') {
    
                dir('/var/lib/jenkins/workspace/10-Tier-Microservice-Application/src/shippingservice') {
                    
                    sh 'docker build -t raghava017/shippingservice:latest .'
                    sh 'docker push raghava017/shippingservice:latest'
                    sh 'docker rmi raghava017/shippingservice:latest'
						}
					}
                }
            }
        }
		
        
    }
}


