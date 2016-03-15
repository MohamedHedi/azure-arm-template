# azure-arm-template

Deploying 10 centos based azure VM

datalab-mesos-master1
datalab-mesos-master2
datalab-mesos-master3
datalab-mesos-slave1
datalab-mesos-slave2
datalab-mesos-slave3
datalab-mesos-middleware1
datalab-mesos-middleware2
datalab-mesos-realtime1
datalab-mesos-realtime2


# install

Switch-AzureMode AzureResourceManager
 
New-AzureResourceGroup -Name 'datalab' `
                       -adminPassword 'mypassword'
                       -TemplateFile 'DeploymentTemplate.json' `
                       -TemplateParameterFile 'DeploymentTemplate.param.json' `
                       -Force -Verbose