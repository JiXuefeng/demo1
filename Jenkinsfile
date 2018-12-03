pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'print demo1 new'
      }
    }
    stage('Report') {
      steps {
        jiraGetComponent(id: 'jenkins', site: 'https://jiraonline.atlassian.net')
        jiraGetProject(idOrKey: 'jenkins', auditLog: true, failOnError: true, site: 'https://jiraonline.atlassian.net')
      }
    }
  }
}