pipeline{
    agent{
        label "agent-helm-k8s"
    }
    stages{
        stage("A"){
            steps{
                echo "=========executing A========"
                script {
                sh '''
                ansible-playbook -i inventories/DEV/hosts.ini playbooks/push-image.yaml
                '''
            }
            }

           
        }
    }
}