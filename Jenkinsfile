node{
    stage('Clone') {
        git 'https://github.com/HichemGue/ansible-jenkins.git
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true, 
          become: true,             
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}
