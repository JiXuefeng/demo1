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
        jiraGetProject(idOrKey: 'jenkins', auditLog: true, failOnError: true, site: 'https://jiraonline.atlassian.net')
      }
    }
  }
}
