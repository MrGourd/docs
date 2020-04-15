# Resource Template Service User Guide

-   [Service Overview]
    -   [RTS](rts.md)
    -   [Advantages](advantages.md)
    -   [Supported Resources](supported-resources.md)
    -   [Constraints](constraints.md)
    -   [Heat Client](heat-client.md)
    -   [User Permissions](user-permissions.md)

-   [Getting Started]
    -   [Creating Resources Using a Template \(Using the Console\)](creating-resources-using-a-template-(using-the-console).md)
    -   [Creating Resources Using a Template \(Using the Heat Client\)](creating-resources-using-a-template-(using-the-heat-client).md)

-   [Operation Guide](operation-guide.md)
-   [Stack Management]
    -   [Preparing a Template or a Template Package]
        -   [Scenarios](scenarios.md)
        -   [Template Package Structure](template-package-structure.md)
        -   [Template File Packaging](template-file-packaging.md)
        -   [Example Template Packages](example-template-packages.md)

    -   [Creating a stack](creating-a-stack.md)
    -   [Viewing Details of a Stack](viewing-details-of-a-stack.md)
    -   [Updating a Stack](updating-a-stack.md)
    -   [Deleting a Stack](deleting-a-stack.md)

-   [Template Syntax]
    -   [Template Structure](template-structure.md)
    -   [Template Version](template-version.md)
    -   [Template Description](template-description.md)
    -   [Parameters](parameters.md)
    -   [Resources](resources.md)
    -   [Outputs](outputs.md)
    -   [Conditions](conditions.md)
    -   [Internal Function](internal-function.md)

-   [Example Templates]
    -   [Creating an ECS](creating-an-ecs.md)
    -   [Creating an ECS and Binding an EIP to the ECS](creating-an-ecs-and-binding-an-eip-to-the-ecs.md)
    -   [Creating an ECS with EVS Disks Mounted](creating-an-ecs-with-evs-disks-mounted.md)
    -   [Creating an ECS Group](creating-an-ecs-group.md)
    -   [Creating an ECS in a Specified Security Group](creating-an-ecs-in-a-specified-security-group.md)
    -   [Creating an AS Group](creating-an-as-group.md)
    -   [Creating a Load Balancer](creating-a-load-balancer.md)
    -   [Creating Network Resources](creating-network-resources.md)

-   [Auditing]
    -   [Key Operations Recorded by CTS](key-operations-recorded-by-cts.md)
    -   [Viewing Audit Logs](viewing-audit-logs.md)

-   [Resource Type Reference]
    -   [OS::Cinder::Volume](os-cinder-volume.md)
    -   [OS::Cinder::VolumeAttachment](os-cinder-volumeattachment.md)
    -   [OS::Heat::AutoScalingGroup](os-heat-autoscalinggroup.md)
    -   [OS::Heat::CloudConfig](os-heat-cloudconfig.md)
    -   [OS::Heat::MultipartMime](os-heat-multipartmime.md)
    -   [OS::Heat::RandomString](os-heat-randomstring.md)
    -   [OS::Heat::ResourceGroup](os-heat-resourcegroup.md)
    -   [OS::Heat::ScalingPolicy](os-heat-scalingpolicy.md)
    -   [OS::Heat::SoftwareComponent](os-heat-softwarecomponent.md)
    -   [OS::Heat::SoftwareConfig](os-heat-softwareconfig.md)
    -   [OS::Heat::SoftwareDeployment](os-heat-softwaredeployment.md)
    -   [OS::Heat::StructuredConfig](os-heat-structuredconfig.md)
    -   [OS::Heat::WaitCondition](os-heat-waitcondition.md)
    -   [OS::Heat::WaitConditionHandle](os-heat-waitconditionhandle.md)
    -   [OS::Neutron::FloatingIP](os-neutron-floatingip.md)
    -   [OS::Neutron::FloatingIPAssociation](os-neutron-floatingipassociation.md)
    -   [OS::Neutron::Net](os-neutron-net.md)
    -   [OS::Neutron::Port](os-neutron-port.md)
    -   [OS::Neutron::Router](os-neutron-router.md)
    -   [OS::Neutron::RouterInterface](os-neutron-routerinterface.md)
    -   [OS::Neutron::SecurityGroup](os-neutron-securitygroup.md)
    -   [OS::Neutron::Subnet](os-neutron-subnet.md)
    -   [OS::Nova::KeyPair](os-nova-keypair.md)
    -   [OS::Nova::Server](os-nova-server.md)
    -   [OS::Nova::ServerGroup](os-nova-servergroup.md)
    -   [OSE::AS::ScalingConfig](ose-as-scalingconfig.md)
    -   [OSE::AS::ScalingGroup](ose-as-scalinggroup.md)
    -   [OSE::AS::ScalingPolicy](ose-as-scalingpolicy.md)
    -   [OSE::CES::Alarm](ose-ces-alarm.md)
    -   [OSE::ELB::LoadBalancer](ose-elb-loadbalancer.md)
    -   [OSE::ELB::Listener](ose-elb-listener.md)
    -   [OSE::ELB::HealthCheck](ose-elb-healthcheck.md)
    -   [OSE::ELB::Member](ose-elb-member.md)
    -   [OSE::ELB::Certificate](ose-elb-certificate.md)
    -   [OS::Neutron::LBaaS::HealthMonitor](os-neutron-lbaas-healthmonitor.md)
    -   [OS::Neutron::LBaaS::Listener](os-neutron-lbaas-listener.md)
    -   [OS::Neutron::LBaaS::LoadBalancer](os-neutron-lbaas-loadbalancer.md)
    -   [OS::Neutron::LBaaS::Pool](os-neutron-lbaas-pool.md)
    -   [OS::Neutron::LBaaS::PoolMember](os-neutron-lbaas-poolmember.md)
    -   [OSE::RDS::Instance](ose-rds-instance.md)
    -   [OSE::VPC::Vpc](ose-vpc-vpc.md)
    -   [OSE::VPC::Subnet](ose-vpc-subnet.md)
    -   [OSE::SFS::Share](ose-sfs-share.md)
    -   [OSE::SFS::ShareAccessRule](ose-sfs-shareaccessrule.md)

-   [FAQ]
    -   [What's the Reason for the Failure to Delete the Stack?](what-s-the-reason-for-the-failure-to-delete-the-stack.md)
    -   [How Are Router Resources in the Native OpenStack Mapped to VPC Resources on the Network Console?](how-are-router-resources-in-the-native-openstack-mapped-to-vpc-resources-on-the-network-console.md)
    -   [How to Obtain the flavor Value of Resource OSE::RDS::Instance?](how-to-obtain-the-flavor-value-of-resource-ose-rds-instance.md)

- 
