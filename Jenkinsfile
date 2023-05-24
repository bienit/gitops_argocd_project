pipeline{
    agent any
    

    stages{

        stage('Git Checkout'){

            steps{

            script{

            git branch: 'main', url: 'https://github.com/bienit/gitops_argocd_project.git'
            }
             }
        } 
        // stage('Clean workspace'){

        //     steps{
        //         script{
        //             cleanWs()
        //         }
        //     }
        // }
    }
}