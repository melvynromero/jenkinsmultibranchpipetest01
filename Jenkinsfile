
import hudson.model.*

node() {

    stage "Begin ... "

    stage "git from repository"
//    git branch: '*/master',  depth:'1' , timeout :'50', shalow: true, noTags: true, changelog: false, credentialsId: '535861b5-0c33-40a0-ba61-b4b71e826d42', poll: false, url: 'http://stash.verizon.com/scm/npdids/iot-integration.git'

// checkout([$class: 'GitSCM', branches: [[name: '*/master']], browser: [$class: 'Stash', repoUrl: 'http://stash.verizon.com/projects/NPDIDS/repos/iot-integration'], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'CloneOption', noTags: true, reference: '', shallow: true, timeout: 60]], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '535861b5-0c33-40a0-ba61-b4b71e826d42', url: 'http://stash.verizon.com/scm/npdids/iot-integration.git']]])

    stage "Ansible Script"

ansiblePlaybook credentialsId: 'df34571d-fb9b-49a6-9ce2-8bdf8ebd39a1', installation: 'Ansible', inventory: 'inventory', playbook: 'provisioning/splunk-setup.yml', sudoUser: null
    stage "... Ending"
}


