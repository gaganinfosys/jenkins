pipeline {
    agent any
    stages{
  stage('Checkout Source') {
      steps {
        git url:'https://github.com/somyaagarwal06/jenkins.git', branch:'main'
      }
    }     
stage('Deploy') {
      steps {
          dir("C:\\Users\\aksuser\\HELM\\courier-stack\\charts"){
          bat "helm list --kubeconfig C:\\Users\\aksuser\\.kube\\config \n\n helm install --generate-name identity --kubeconfig C:\\Users\\aksuser\\.kube\\config \n kubectl get pods --kubeconfig C:\\Users\\aksuser\\.kube\\config"
    }
      }
}
}
}
