pipeline {
  agent any
  
  parameters {
    gitParameter branchFilter: '.*', defaultValue: 'develop', name: 'GIT_BRANCH', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH'
  }
  
  stages {
    stage('Checkout') {
      steps {
        checkout([
          $class: 'GitSCM',
          branches: [[name: "${params.GIT_BRANCH}"]],
          userRemoteConfigs: [[
            url: 'https://github.com/sPoojarySujith/Jenkins_FindFile.git'
          ]]
        ])
      }
    }
    
    // Add your build stages here
    
  }
}
