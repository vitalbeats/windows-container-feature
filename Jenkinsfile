pipeline {
  agent {
    kubernetes {
      defaultContainer 'jnlp'
      yamlFile 'agent-pod.yaml'
    }
  }

  stages {
    stage('Ansible Lint') {
      steps {
        container('ansible-lint') {
          sh 'ansible-lint -p . > ansible.report || true'
          recordIssues tool: ansibleLint(pattern: 'ansible.report'), qualityGates: [[threshold: 1, type: 'TOTAL', unstable: false]]
        }
      }
    }
  }
}
