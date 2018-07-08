#!groovy
@Library('OpsTree-DevOps@master') _

node {
   spring {
      git_url     = "https://github.com/navdeepmanchanda/pipeline.git"
      branch      = "master"
      credentials = "git"
      maven_goals = "clean install -Dmaven.test.skip=true"
      maven_test_goals = "test -Dmaven.test.failure.ignore=true"
      pom_path    = "EmployeeAutomation/pom.xml"
   }
}
