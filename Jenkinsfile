pipeline {
    agent any
    stages {
        stage('Install ansible roles') {
            steps {
                sh 'ansible-galaxy install --force  -r requirements.yml --roles-path roles'
            }
        }
      
      stage('Run playbook') { 
        steps{
            sh 'ansible-playbook main.yml --tags "first-test" -vvv'
            sh 'ansible-playbook main.yml --tags "second-test" -vvv'
            }
        }
    }
   
}
