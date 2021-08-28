pipeline { 
    agent any 
    stages {
        
        stage('Git Project checkout') {
        steps {
               git branch: 'master', url: 'https://github.com/Anirudhbly/Ansible-integration-Jenkins-install-Apachewebserver.git'  
          }
        }
        
        stage('Execute Ansible Playbook') { 
            steps {
                ansiblePlaybook disableHostKeyChecking: true, installation: 'Ansible', inventory: 'dev.inv', playbook: 'apache.yml'                
                }
            }
        }
}
