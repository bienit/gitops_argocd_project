pipeline{
    agent any
    environment{
        DOCKERHUB_USERNAME = "111188889999"
        APP_NAME = "gitops-argo-app"
        IMAGE_TAG = "${BUILD_NUMBER}"
        IMAGE_NAME = "${DOCKERHUB_USERNAME}"+ "/" + "${APP_NAME}"
        REGISTRY_CREDS = 'dockerhub'
    }

    stages{
        


        stage('Git Checkout'){

        steps{

            script{
                git credentialsId: 'github',
                url: 'https://github.com/bienit/gitops_argocd_project.git',
                branch: 'main'
                }
            }
            }
    } 

}
