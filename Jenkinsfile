pipeline {
  agent {
    node {
      label 'aws-test'
    }

  }
  stages {
    stage('dev') {
      steps {
        cfnValidate(file: 'EC2ElasticIPSample', url: 'https://s3-us-west-2.amazonaws.com/cloudformation-templates-us-west-2/EIP_With_Association.template')
        sh 'echo "hello word"'
      }
    }
    stage('pre') {
      steps {
        sh 'echo "hello word"'
      }
    }
    stage('') {
      steps {
        sh 'echo "hello"'
      }
    }
  }
}