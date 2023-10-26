stage('test parallel jobs') {
  def jobs = [:]

  jobs["j1"] = {
    parallel([
      c1: {
        echo "hello from c1"
      },
      c2: {
        echo "hello from c2"
      }
    ])
  }

  jobs["j2"] = {
    node('ecs-rockylinux8_openjdk17_jenkins_agent') {
      sh "hostname"
    }
  }

  parallel(jobs)
}
