pipleline{
    agent any
    stages {
        stage('Execute Ansible Playbook'){
            steps{
                ansiblePlaybook credentialsId: 'private-key', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'dev.inv', playbook: 'apache.yml'
            }
        }
   }
}
