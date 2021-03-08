pipeline {
    agent any
    stages {
        stage('Install ansible roles') {
            steps {
                sh 'echo "hello"'
                sh 'ansible-galaxy install --force  -r requirements.yml --roles-path roles; ansible-playbook main.yml --tags "first-test" -vvv'
                //sh 'ansible-playbook main.yml --tags "first-test" -vvv'
            }
        }
      
     // stage('Run playbook') { 
        //steps{
          //  sh 'ansible-playbook main.yml --tags "first-test" -vvv'
         // }
        //}
    }
   
}
