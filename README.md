# Observability platform engineer test task

I am pleased to say that we are ready to move on to the next stage in our recruitment process and send you a test task, please find it below. We do not have any specific deadline for it, but we would appreciate it if you let us know approximately how long it will take you to complete. Also, feel free of course to ask questions should you have any. Once you are done, please send the solution back to me.

Create code for your favorite automation tool (Chef, Ansible, Bash, Terraform, CloudFormation etc.) to deploy Observability stack consisting of Grafana and Prometheus on platform of your choice (AWS, OpenStack, VirtualBox, QEMU, Docker, Vagrant or anything else).
Commit the code to a git repository (Github, Bitbucket, etc.) and provide a link to the repository as a solution.

Requirements:
Software versions: any supported version is okay.
Operating system: any supported version of Debian, Ubuntu, CentOS or Fedora.
If using Docker -- write your own Dockerfiles, do not use containers from Docker Hub!
All the servers can reside in the same local network.
End solution should have a working dashboard in Grafana with node metrics from Grafana and/or Prometheus machine or even from your host machine. https://github.com/prometheus/node_exporter

Minimal solution: code to install and configure:
- Grafana server
  - Grafana frontend accessible
  - Working Prometheus datasource
  - Dashboard with CPU/Memory/Filesystem metrics
- Prometheus server
  - Prometheus server running
  - Prometheus frontend accessible
  - Prometheus scraping metrics from at least one node exporter (can also be your host machine)

It is fine to leave some steps manual, however, you'll get the maximum score if the process is as automated as possible.
Please include short notes in README.md of your Git repository with instructions on how to use your code and a description of manual steps if any.

Bonus tasks:
- Automate virtual machine and/or container creation and orchestration
  - Can use the same or some other automation framework
- Add alerting to your Grafana dashboard
  - Alerts can be configured to sent to slack / email or any other notification channel of your choice
- Describe backup approach for all components (free text)
- Use standard HTTP ports and set up a TLS for all services
  - Self-signed certificates are okay
