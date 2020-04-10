# User Guide

-   [Overview]
    -   [What Is Image Management Service?](what-is-image-management-service.md)
    -   [Supported OSs]
        -   [OSs Supported by Different Types of ECSs](oss-supported-by-different-types-of-ecss.md)
        -   [Formats and OSs Supported for External Image Files](formats-and-oss-supported-for-external-image-files.md)

    -   [Basic Concepts]
        -   [Region and AZ](region-and-az.md)
        -   [Common Image Formats](common-image-formats.md)

    -   [Related Services](related-services.md)

-   [Creating a Private Image]
    -   [Introduction](introduction.md)
    -   [Creating a System Disk Image from a Windows ECS](creating-a-system-disk-image-from-a-windows-ecs.md)
    -   [Creating a System Disk Image from a Linux ECS](creating-a-system-disk-image-from-a-linux-ecs.md)
    -   [Creating a Windows System Disk Image from an External Image File]
        -   [Overview](overview-(windows).md)
        -   [Preparing an Image File](preparing-an-image-file-(windows).md)
        -   [Uploading an External Image File](uploading-an-external-image-file-(windows).md)
        -   [Registering an External Image File as a Private Image](registering-an-external-image-file-as-a-private-image-(windows).md)
        -   [Creating a Windows ECS from an Image](creating-a-windows-ecs-from-an-image.md)

    -   [Creating a Linux System Disk Image from an External Image File]
        -   [Overview](overview-(linux).md)
        -   [Preparing an Image File](preparing-an-image-file-(linux).md)
        -   [Uploading an External Image File](uploading-an-external-image-file-(linux).md)
        -   [Registering an External Image File as a Private Image](registering-an-external-image-file-as-a-private-image-(linux).md)
        -   [Creating a Linux ECS from an Image](creating-a-linux-ecs-from-an-image.md)

    -   [Creating a BMS System Disk Image](creating-a-bms-system-disk-image.md)
    -   [Creating a Data Disk Image from an ECS Data Disk](creating-a-data-disk-image-from-an-ecs-data-disk.md)
    -   [Creating a Data Disk Image from an External Image File](creating-a-data-disk-image-from-an-external-image-file.md)
    -   [Creating a Full-ECS Image from an ECS](creating-a-full-ecs-image-from-an-ecs.md)
    -   [Creating a Full-ECS Image from a CSBS Backup](creating-a-full-ecs-image-from-a-csbs-backup.md)

-   [Managing Private Images]
    -   [Modifying Image Information](modifying-image-information.md)
    -   [Creating an ECS from an Image](creating-an-ecs-from-an-image.md)
    -   [Deleting Images](deleting-images.md)
    -   [Sharing Images]
        -   [Overview](sharing-images-overview.md)
        -   [Obtaining the Project ID](obtaining-the-project-id.md)
        -   [Sharing Specified Images](sharing-specified-images.md)
        -   [Accepting or Rejecting Shared Images](accepting-or-rejecting-shared-images.md)
        -   [Rejecting Accepted Images](rejecting-accepted-images.md)
        -   [Accepting Rejected Images](accepting-rejected-images.md)
        -   [Stopping Sharing Images](stopping-sharing-images.md)
        -   [Adding Tenants Who Can Use Shared Images](adding-tenants-who-can-use-shared-images.md)
        -   [Deleting Image Recipients Who Can Use Shared Images](deleting-image-recipients-who-can-use-shared-images.md)

    -   [Exporting Images](exporting-images.md)
    -   [Optimizing a Windows Private Image]
        -   [Optimization Process](optimization-process-(windows).md)
        -   [Viewing the Virtualization Type of a Windows ECS](viewing-the-virtualization-type-of-a-windows-ecs.md)
        -   [Obtaining Required Software Packages](obtaining-required-software-packages.md)
        -   [Installing the PV Driver](installing-the-pv-driver.md)
        -   [Installing UVP VMTools](installing-uvp-vmtools.md)
        -   [Clearing System Logs](clearing-system-logs-(windows).md)

    -   [Optimizing a Linux Private Image]
        -   [Optimization Process](optimization-process-(linux).md)
        -   [Viewing the Virtualization Type of a Linux ECS](viewing-the-virtualization-type-of-a-linux-ecs.md)
        -   [Uninstalling the PV Driver from a Linux ECS](uninstalling-the-pv-driver-from-a-linux-ecs.md)
        -   [Changing the Disk Identifier in the GRUB Configuration File to UUID](changing-the-disk-identifier-in-the-grub-configuration-file-to-uuid.md)
        -   [Changing the Disk Identifier in the fstab File to UUID](changing-the-disk-identifier-in-the-fstab-file-to-uuid.md)
        -   [Installing Native Xen and KVM Drivers](installing-native-xen-and-kvm-drivers.md)
        -   [Clearing System Logs](clearing-system-logs-(linux).md)

    -   [Encrypting Images]
        -   [Overview](encrypting-images-overview.md)
        -   [Creating Encrypted Images](creating-encrypted-images.md)

    -   [Replicating Images](replicating-images.md)
    -   [Tagging an Image](tagging-an-image.md)
    -   [Exporting Image Information](exporting-image-information.md)
    -   [Auditing Key Operations]
        -   [Key IMS Operations Recorded by CTS](key-ims-operations-recorded-by-cts.md)
        -   [Viewing Traces](viewing-traces.md)

    -   [Converting the Image Format](converting-the-image-format.md)
    -   [Quickly Importing an Image File]
        -   [Overview](quickly-importing-an-image-file-overview.md)
        -   [Quickly Importing an Image File \(Linux\)](quickly-importing-an-image-file-(linux).md)
        -   [Quickly Importing an Image File \(Windows\)](quickly-importing-an-image-file-(windows).md)


-   [Windows Operations]
    -   [Setting the NIC to DHCP \(Windows\)](setting-the-nic-to-dhcp-(windows).md)
    -   [Enabling Remote Desktop Connection](enabling-remote-desktop-connection.md)
    -   [Installing and Configuring Cloudbase-Init](installing-and-configuring-cloudbase-init.md)
    -   [Running Sysprep](running-sysprep.md)
    -   [Installing Special Windows Drivers](installing-special-windows-drivers.md)

-   [Linux Operations]
    -   [Setting the NIC to DHCP \(Linux\)](setting-the-nic-to-dhcp-(linux).md)
    -   [Deleting Files in the Network Rule Directory](deleting-files-in-the-network-rule-directory.md)
    -   [Installing Cloud-Init](installing-cloud-init.md)
    -   [Configuring Cloud-Init](configuring-cloud-init.md)
    -   [Installing Special Linux Drivers](installing-special-linux-drivers.md)
    -   [Detaching Data Disks from an ECS](detaching-data-disks-from-an-ecs.md)
    -   [Configuring Console Logging](configuring-console-logging.md)

-   [FAQs]
    -   [General FAQs]
        -   [How Do I Select an Image?](how-do-i-select-an-image.md)

    -   [Image Creation]
        -   [Image Creation FAQs](image-creation-faqs.md)
        -   [Can I Use Images in Formats Other Than Those Specified in This Document?](can-i-use-images-in-formats-other-than-those-specified-in-this-document.md)
        -   [How Do I Create a Full-ECS Image Using an ECS That Has a Spanned Volume?](how-do-i-create-a-full-ecs-image-using-an-ecs-that-has-a-spanned-volume.md)
        -   [Why Is Sysprep Required for Creating a Private Image from a Windows ECS?](why-is-sysprep-required-for-creating-a-private-image-from-a-windows-ecs.md)
        -   [What Do I Do If I Cannot Create an Image in the ZVHD2 Format Using an API?](what-do-i-do-if-i-cannot-create-an-image-in-the-zvhd2-format-using-an-api.md)
        -   [What Is the Impact If I Do Not Pre-configure an ECS Used to Create a Private Image?](what-is-the-impact-if-i-do-not-pre-configure-an-ecs-used-to-create-a-private-image.md)
        -   [What Can I Do If I Configure an Incorrect OS or System Disk Size During Private Image Registration Using an Image File?](what-can-i-do-if-i-configure-an-incorrect-os-or-system-disk-size-during-private-image-registration-u.md)
        -   [Why Does the Error Message Displayed on Task Center Indicates That the System Disk Size of the External Image File Exceeds the Maximum System Disk Size When a VHD Image File Failed to Be Uploaded?](why-does-the-error-message-displayed-on-task-center-indicates-that-the-system-disk-size-of-the-exter.md)

    -   [Image Optimization]
        -   [Must I Install the Guest OS Driver on ECSs?](must-i-install-the-guest-os-driver-on-ecss.md)
        -   [What Changes Will Be Made to an Image File Used for Registering a Private Image?](what-changes-will-be-made-to-an-image-file-used-for-registering-a-private-image.md)
        -   [What Initial Configuration Needs to Be Performed on the ECS, BMS, or Image File Before It Is Used to Create an Image?](what-initial-configuration-needs-to-be-performed-on-the-ecs-bms-or-image-file-before-it-is-used-to-c.md)
        -   [What Do I Do If the Initial Configurations of a Windows External Image File Are Not Completed Before the File Is Exported?](what-do-i-do-if-the-initial-configurations-of-a-windows-external-image-file-are-not-completed-before.md)
        -   [What Do I Do If the Initial Configurations of a Linux External Image File Are Not Completed Before the File Is Exported?](what-do-i-do-if-the-initial-configurations-of-a-linux-external-image-file-are-not-completed-before-t.md)
        -   [How Do I Set NIC Multi-Queue Feature of an Image?](how-do-i-set-nic-multi-queue-feature-of-an-image.md)
        -   [How Do I Optimize a System Disk Image So That It Can Be Used to Create ECSs Quickly?](how-do-i-optimize-a-system-disk-image-so-that-it-can-be-used-to-create-ecss-quickly.md)
        -   [What Is the Cause of the Failure to Install the Guest OS Driver on a Windows ECS?](what-is-the-cause-of-the-failure-to-install-the-guest-os-driver-on-a-windows-ecs.md)

    -   [Image Management]
        -   [Image Sharing FAQs](image-sharing-faqs.md)
        -   [Encrypted Image FAQs](encrypted-image-faqs.md)
        -   [Can I Use Private Images of Other Tenants?](can-i-use-private-images-of-other-tenants.md)

    -   [Cloud-Init Operations]
        -   [What Do I Do If Injecting the Key or Password Using Cloud-Init Fails After NetworkManager Is Installed?](what-do-i-do-if-injecting-the-key-or-password-using-cloud-init-fails-after-networkmanager-is-install.md)
        -   [How Do I Install growpart for SUSE 11 SP4?](how-do-i-install-growpart-for-suse-11-sp4.md)
        -   [How Do I Configure a Linux Private Image That Can Automatically Expand Its Root Partition?](how-do-i-configure-a-linux-private-image-that-can-automatically-expand-its-root-partition.md)

    -   [ECS]
        -   [How Do I Install the NVIDIA Driver on a P1 ECS?](how-do-i-install-the-nvidia-driver-on-a-p1-ecs.md)
        -   [Can an ECS Created from a Private Image Have Different Hardware Specifications from the ECS Used to Create the Private Image?](can-an-ecs-created-from-a-private-image-have-different-hardware-specifications-from-the-ecs-used-to.md)
        -   [Can I Specify the System Disk Size When Create an ECS Using an Image?](can-i-specify-the-system-disk-size-when-create-an-ecs-using-an-image.md)
        -   [How Do I Delete Redundant Network Connections to a Windows ECS?](how-do-i-delete-redundant-network-connections-to-a-windows-ecs.md)
        -   [What Do I Do If No Partition Is Found During the Startup of an ECS Created from an Imported Private Image?](what-do-i-do-if-no-partition-is-found-during-the-startup-of-an-ecs-created-from-an-imported-private.md)
        -   [What Do I Do If the Disks of an ECS Created from a CentOS Image Cannot Be Found?](what-do-i-do-if-the-disks-of-an-ecs-created-from-a-centos-image-cannot-be-found.md)
        -   [What Should I Do If an ECS Starts Slowly?](what-should-i-do-if-an-ecs-starts-slowly.md)
        -   [What Do I Do If a Windows 7 ECS Equipped with an Intel 82599 NIC Reports an Error in SR-IOV Scenarios?](what-do-i-do-if-a-windows-7-ecs-equipped-with-an-intel-82599-nic-reports-an-error-in-sr-iov-scenario.md)
        -   [How Do I Resolve the Issue That an ECS Created from a Windows Image Fails to Start When I Have Selected Enable Automatic Configuration During Image Registration?](how-do-i-resolve-the-issue-that-an-ecs-created-from-a-windows-image-fails-to-start-when-i-have-selec.md)
        -   [What Do I Do If an Exception Occurs When I Start an ECS Created from an Image Using the UEFI Boot Mode?](what-do-i-do-if-an-exception-occurs-when-i-start-an-ecs-created-from-an-image-using-the-uefi-boot-mo.md)


-   [Glossary](glossary.md)

