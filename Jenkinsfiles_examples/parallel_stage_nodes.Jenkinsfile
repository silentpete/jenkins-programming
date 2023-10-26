stage('test parallel nodes') {
  def nodes = [:]

  nodes["n1"] = {
    node('ecs-jenkins_agent') {
      sh "hostname"
    }
  }

  nodes["n2"] = {
    node('ecs-rockylinux8_openjdk17_jenkins_agent') {
      sh "hostname"
    }
  }

  parallel(nodes)
}
