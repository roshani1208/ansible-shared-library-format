pipeline {
    agent any
    stages {
        stage('Install ansible roles') {
            steps {
                sh 'ansible-galaxy install --force  -r requirements.yml --roles-path .'
            }
        }
      
      stage('Run playbook') { 
        steps{
            sh 'ansible-playbook main.yml -vvv'
            }
        }
    }
   
}
