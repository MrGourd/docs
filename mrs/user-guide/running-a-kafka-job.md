# Running a Kafka Job<a name="EN-US_TOPIC_0221415050"></a>

You can submit programs developed by yourself to MRS to execute them, and obtain the results. This topic describes how to generate and consume messages in a Kafka topic.

Currently, Kafka jobs cannot be submitted on the GUI. You can submit them in the background.

## Submitting a Job in the Background<a name="section12299175615451"></a>

1.  Log in to the MRS management console.
2.  Choose  **Clusters \> Active Clusters**, select a running cluster, and click its name to switch to the cluster details page.
3.  On the cluster details page, click  **View**  next to  **Cluster Manager**  to access MRS Manager. For details, see  [Accessing MRS Manager](accessing-mrs-manager.md).
4.  On the MRS cluster details page, choose  **Services**  \>  **ZooKeeper**  \>  **Instance**  to query the IP addresses of ZooKeeper instances. Record any IP address of a ZooKeeper instance.
5.  Choose  **Services**  \>  **Kafka**  \>  **Instance**  to query the IP addresses of Kafka instances. Record any IP address of a Kafka instance.
6.  Log in to any Master node. For details, see  [Logging In to a Master Node](logging-in-to-a-master-node.md).
7.  Run the following command to initialize environment variables:

    **source /opt/client/bigdata\_env**

8.  If the Kerberos authentication is enabled for the current cluster, run the following command to authenticate the user. If the Kerberos authentication is disabled for the current cluster, skip this step.

    **kinit** **_MRS cluster user_**

    Example:  **kinit admin**

9.  Run the following command to create a Kafka topic:

    **kafka-topics.sh --create --zookeeper <IP address of the ZooKeeper role instance:2181/kafka\> --partitions 2 --replication-factor 2 --topic <Topic name\>**

10. Produce messages in a topic test.

    Run  **kafka-console-producer.sh --broker-list <IP address of the ZooKeeper role instance:9092\> --topic <Topic name\> --producer.config /opt/client/Kafka/kafka/config/producer.properties**.

    Enter the specified content as a message generated by the producer, and press  **Enter**  to send the message. To end message production, press  **Ctrl+C**  to exit.

11. Consume messages in the topic test.

    **kafka-console-consumer.sh --topic <Topic name\> --bootstrap-server <IP address of the ZooKeeper role instance:9092\> --new-consumer --consumer.config /opt/client/Kafka/kafka/config/consumer.properties**

    >![](public_sys-resources/icon-note.gif) **NOTE:**   
    >If Kerberos authentication is enabled in the cluster, change the port number 9092 to 21007 when running the preceding two commands. For details, see  [List of Open Source Component Ports](list-of-open-source-component-ports.md).  

