pipeline{
  agent{label 'slave'}
  parameters{
    choice(name:'VERSION', choices:['1.0','1.1','1.2'], description:'version to deploy')
  }
  stages{
    stage("build"){
      steps{
        echo "building the application war file with mentioned version ${params.VERSION}"
      }
    }
    stage("test"){
      steps{
        echo "performing tests"
        echo "performed and all tests successful"
      }
    }
    stage("deploy"){
      steps{
        echo "built version ${params.VERSION} deployed successfully"
      }
    }
  }
}
