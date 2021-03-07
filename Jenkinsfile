pipeline {
    agent any
    stages {
        stage('Install ansible roles') {
            steps {
                sh 'ansible-galaxy install -r requirements.yml'
            }
        }
      
      stage('Run playbook') { 
        steps{
            sh 'ansible-playbook main.yml -vvv'
            }
        }
    }
   
}
