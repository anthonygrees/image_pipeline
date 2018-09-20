pipeline {
  agent any
  stages {
    stage('Create PR') {
      steps {
        echo 'Create PR'
      }
    }
    stage('Get Base ISO') {
      steps {
        echo 'Test'
      }
    }
    stage('Install Chef Agent') {
      steps {
        echo 'Test'
      }
    }
    stage('Load Policyfile Archive') {
      steps {
        echo 'Test'
      }
    }
    stage('chef-client -z policyfile_archive') {
      parallel {
        stage('Harden OS') {
          steps {
            echo 'test'
          }
        }
        stage('Patch OS') {
          steps {
            echo 'test'
          }
        }
        stage('Audit OS') {
          steps {
            echo 'test'
          }
        }
      }
    }
    stage('Kitchen Integration Test') {
      parallel {
        stage('OS Tests') {
          steps {
            echo 'test'
          }
        }
        stage('Middleware Test') {
          steps {
            echo 'test'
          }
        }
      }
    }
    stage('Remove Chef Agent') {
      steps {
        echo 'Test'
      }
    }
    stage('New versioned Base Image') {
      steps {
        echo 'Test'
      }
    }
    stage('Publish Image') {
      steps {
        echo 'Publish to Artifactory'
      }
    }
    stage('Commit to Master') {
      steps {
        echo 'test'
      }
    }
  }
}
