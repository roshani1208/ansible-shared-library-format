pipeline {
    agent any
    stages {
        stage('Install ansible roles') {
            steps {
                sh 'ansible-galaxy install --force  -r requirements.yml --roles-path .'
                sh 'ansible-playbook main.yml --tags "first-test" -vvv'
            }
        }
      
     // stage('Run playbook') { 
        //steps{
          //  sh 'ansible-playbook main.yml --tags "first-test" -vvv'
         // }
        //}
    }
   
}
