---
author: jsntcy
---

# list-with-note
    
1. Copy the Hive JDBC drivers from your HDInsight cluster.
   
    * For **Linux-based HDInsight**, use the following steps to download the required jar files.    
    * For **Windows-based HDInsight**, use the following steps to download the jar files.
     
        1. From the Azure portal, select your HDInsight cluster, and then select the **Remote Desktop** icon.
        
            ![Remote Desktop icon](./media/hdinsight-connect-hive-jdbc-driver/remotedesktopicon.png)

        2. On the Remote Desktop blade, use the **Connect** button to connect to the cluster. If the Remote Desktop is not enabled, use the form to provide a user name and password, then select **Enable** to enable Remote Desktop for the cluster.
        
            ![Remote desktop blade](./media/hdinsight-connect-hive-jdbc-driver/remotedesktopblade.png)
        
            After selecting **Connect**, a .rdp file will be downloaded. Use this file to launch the Remote Desktop client. When prompted, use the user name and password you entered for Remote Desktop access.

        3. Once connected, copy the following files from the Remote Desktop session to your local machine. Put them in a local directory named `hivedriver`.
        
            * C:\apps\dist\hive-0.14.0.2.2.9.1-7\lib\hive-jdbc-0.14.0.2.2.9.1-7-standalone.jar
            * C:\apps\dist\hadoop-2.6.0.2.2.9.1-7\share\hadoop\common\hadoop-common-2.6.0.2.2.9.1-7.jar
            * C:\apps\dist\hadoop-2.6.0.2.2.9.1-7\share\hadoop\common\lib\hadoop-auth-2.6.0.2.2.9.1-7.jar
          
          
            > [!NOTE]
            > The version numbers included in the paths and file names may be different for your cluster.


        4. Disconnect the Remote Desktop session once you have finished copying the files.
