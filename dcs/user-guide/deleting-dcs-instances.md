# Deleting DCS Instances<a name="en-us_topic_0054235819"></a>

## Scenario<a name="section8135151"></a>

On the DCS console, you can delete one or multiple DCS instances at a time. You can also delete all instance creation tasks that have failed to run.

>![](public_sys-resources/icon-notice.gif) **NOTICE:** 
>After a DCS instance is deleted, data from the instance will also be deleted without backup.

## Prerequisites<a name="section6107499"></a>

-   The DCS instances you want to delete have been created.
-   The DCS instances you want to delete are in the** Running**,  **Faulty**  state.

## Deleting DCS Instances<a name="section28432151594"></a>

1.  Log in to the management console.
2.  Click  ![](figures/project.png) in the upper left corner of the management console and select a region and a project.
3.  Click  **Service List**, and choose **Database** \> **Distributed Cache Service**  to launch the DCS console.
4.  In the navigation pane, choose  **Cache Manager**.
5.  Choose instances to delete.

    -   To delete a single instance, choose  **Operation** \> **More** \> **Delete**  in the same row as the instance.
    -   To delete multiple instances, select the instances to delete and click  **Delete**  above the instance list.

    DCS instances in the  **Creating**,** **or  **Restarting**  state cannot be deleted.

6.  Click **Yes **to confirm that you want to delete the instances.

    It takes 1 to 30 minutes to delete DCS instances.


## Deleting Instance Creation Tasks That Have Failed to Run<a name="section61981843115915"></a>

1.  Log in to the management console.
2.  Click  ![](figures/project.png) in the upper left corner of the management console and select a region and a project.
3.  Click  **Service List**, and choose **Database** \> **Distributed Cache Service**  to launch the DCS console.
4.  In the navigation pane, choose  **Cache Manager**.

    If there are DCS instances that have failed to be created,  **Instance Creation Failures**  is displayed above the instance list.

5.  Click the icon or the number of failed tasks next to  **Instance Creation Failures**.

    The  **Instance Creation Failures**  dialog box is displayed.

6.  Choose failed instance creation tasks to delete.
    -   To delete a single failed task, click  **Delete**  in the same row as the task.
    -   To delete all failed tasks, click  **Delete All **above the task list.


