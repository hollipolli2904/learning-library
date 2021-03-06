# Connect to an Oracle Database in a Docker Container
## Before You Begin

This lab walks you through the steps to connect to an Oracle Database running in a Docker container on an Oracle Cloud Compute instance. You can connect the Oracle Database instance using any client you wish. In this lab, you'll connect using Oracle SQLDeveloper.

### What Do You Need?

* An Oracle Cloud paid account or free trial. To sign up for a trial account with $300 in credits for 30 days, click [here]http://oracle.com/cloud/free).
* SSH keys
* A Docker container running Oracle Database 19c
* * An open port (1521) on your Oracle Cloud Virtual Cloud Network (VCN)
* [Oracle SQL Developer](https://www.oracle.com/tools/downloads/sqldev-downloads.html)

## **STEP 1**: Create a connection through SQL Developer

1. Launch Oracle SQL Developer and select **New Connection** (the green + sign).

  ![](images/sd-create-connection.png " ")

2. In the New / Select Database Connection window, enter the following information:
     * In the **Name** field, enter **DockerDB** as the name of this connection.
     * In the **Username** field, enter **sys**.
     * In the **Password** field, enter the password (`LetsDocker`) for the SYS account.
     * Select **SYSDBA** from the **Role** drop down list.
     * Check the **Save Password** checkbox.
     * In the **Hostname** field, enter your Oracle Compute instance Public IP address.
     * Click **Service name** and enter **ORCLPDB1**.

   ![](images/sd-new-connection.png " ")

3. Click **Test** to check your connection. You see a Success message in the **Status** field.
4. Click **Save** to save your connection details and then click **Connect**.

5. You now have a connection to your Oracle VM Database system, and you can expand the connection and Tables.

  ![](images/sd-connected.png " ")

  You may now proceed to the next lab.

## Want to Learn More?

* [Oracle SQL Developer Documentation](https://docs.oracle.com/en/database/oracle/sql-developer/)
* [Oracle Cloud Infrastructure: Connecting to an DB System](https://docs.cloud.oracle.com/en-us/iaas/Content/Database/Tasks/connectingDB.htm)

## Acknowledgements
* **Author** - Gerald Venzl, Master Product Manager, Database Development
* **Adapted for Cloud by** -  Tom McGinn, Learning Architect, Database User Assistance
* **Last Updated By/Date** - Tom McGinn, March 2020

See an issue?  Please open up a request [here](https://github.com/oracle/learning-library/issues).   Please include the workshop name and lab in your request. 
