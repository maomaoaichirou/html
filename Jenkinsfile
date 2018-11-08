pipeline {
  agent {
    node {
      label 'aws-test'
    }

  }
  stages {
    stage('') {
      steps {
        cfnValidate(file: 'EC2ElasticIPSample', url: 'https://s3-us-west-2.amazonaws.com/cloudformation-templates-us-west-2/EIP_With_Association.template')
      }
    }
  }
}