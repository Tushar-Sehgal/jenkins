pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        // Use a build automation tool Maven to compile and package the code
        echo "Tool Used: Maven"
        echo "Maven is a tool that automates the creation of Java programmes. The structure and dependencies of our project are defined by a project object model (POM), and Maven uses plugins to carry out operations like code compilation, test execution, and programme packaging. We can accomplish both of these things while saving time on various projects."
      }
      post {
        success {
          // Use the Email Extension Plugin to send notification emails
          mail to: "abliscence@gmail.com",
          subject: "Build Status Email",
          body: "Build was successful!"
        }
      }
    }
    stage('Unit and Integration Tests') {
      steps {
        // Use test automation tool Emma to run unit tests and integration tests
        echo "Tool Used: Emma"
        echo "Emma is a tool used in Java programming for unit and integration testing. By keeping track of how much of the code is being tested, it helps to ensure that it functions correctly and is bug-free. Having thorough tests and testing as much of our code as possible can help find bugs earlier and cut down on the amount of time needed for debugging. As a result of Emma's widespread use in the Java community, it is a dependable tool for testing across various projects."
      }
      post {
        success {
          // Use the Email Extension Plugin to send notification emails
          mail to: "abliscence@gmail.com",
          subject: "Unit and Integration Test Email",
          body: "Unit and integration test was successful!"
        }
      }
    }
    stage('Code Analysis') {
      steps {
        // Use a code analysis tool Checkstyle to analyze the code and ensure it meets industry standards
        echo "Tool Used: Checkstyle"
        echo "Java programmers can analyse code using a tool called Checkstyle. Checking our code against a set of predefined rules and guidelines enables us to make sure that it is readable, maintainable, and adheres to coding standards. Additionally, it increases the readability and maintainability of our code and enables us to identify potential problems early. As a result of its widespread use in the Java community, our coding standards are reliable and consistent across numerous projects."
      }
    }
    stage('Security Scan') {
      steps {
        // Use a security scanning tool Probley to perform a security scan on the code and identify any vulnerabilities
        echo "Tool Used: Probley"
        echo "In web applications, Probley is a tool used for security scans. By scanning the code of web applications and identifying any potential security issues, it helps to ensure that they are safe and free of vulnerabilities that could be used by attackers. Additionally, it lessens the likelihood of a security breach by identifying potential security issues early on. Web developers frequently use Probley to make sure that the security scanning procedure is dependable and consistent."
      }
      post {
        success {
          // Use the Email Extension Plugin to send notification emails
          mail to: "abliscence@gmail.com",
          subject: "Security Scan Status Email",
          body: "Security scan was successful!"
        }
      }
    }
    stage('Deploy to Staging') {
      steps {
        // Use a deployment tool such as AWS CodeDeploy to deploy the application to a staging server
        echo "Tool Used: AWS EC2"
        echo "In staging environments, where changes can be made without having an impact on actual users, we test our applications in a setting that is similar to production. By offering virtual servers (referred to as instances) that can be used to deploy our applications to Staging, AWS EC2 streamlines this process. We can test our application in the Staging environment after it has been deployed to the EC2 instance to make sure it performs as expected. Our application is deployed to Staging using AWS EC2, which enables us to identify potential problems early and lowers the risk of introducing bugs or other problems into production. AWS EC2 also offers a dependable and expandable platform for the deployment and testing of applications."
      }
    }
    stage('Integration Tests on Staging') {
      steps {
        // Use test automation tool Selenium to run integration tests on the staging environment
        echo "Tool Used: Selenium"
        echo "Selenium is used in automation to simulate user interactions with a web browser to automate repetitive tasks such as testing, web scraping, and web application monitoring."
      }
      post {
        success {
          // Use the Email Extension Plugin to send notification emails
          mail to: "abliscence@gmail.com",
          subject: "Integration Tests on Staging Status Email",
          body: "Integration test was successful!"
        }
      }
    }
    stage('Deploy to Production') {
      steps {
        // Use a deployment tool such as AWS CodeDeploy to deploy the application to a production server
        echo "Tool Used: AWS CodeDeploy"
        echo "AWS CodeDeploy is used in automation to deploy applications automatically to EC2 instances or on-premises servers, ensuring consistent deployment of new code changes across environments."
        echo "Testing Automated Build..."
      }
    }
  }
}
