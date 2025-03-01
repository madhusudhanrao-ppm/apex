# Import the Social Media Application

## Introduction

In this lab, you explore the integration of a Social Media application with OCI AI vision.

You can download the catch up scripts of the Social Media Application [here](https://objectstorage.us-ashburn-1.oraclecloud.com/p/LNAcA6wNFvhkvHGPcWIbKlyGkicSOVCIgWLIu6t7W2BQfwq2NSLCsXpTL9wVzjuP/n/c4u04/b/livelabsfiles/o/developer-library/APEX_Social_Media_HOL_FINAL.zip).


Estimated Time: 15 Minutes

### Objectives
In this lab, you:

- Import the Social Media Application
- Change the Authentication Type in Social Media Application
- Add a Column to the Table using Object Browser

## Task 1: Import the Social Media Application

1. On the Workspace home page, click the **App Builder** icon.
   On the App Builder home page, click **Import**.

    ![Click Import](images/import0.png " ")

2. The Import dialog displays. Download the Export File of the APEX Social Medial Application and then perform the following steps.
    - Drag and drop, or navigate to the file.

    - File Type: Indicate the type of export file to be imported. Select **Application, Page, or Component Export**.

    - File Character Set: Verify that the File Character Set is correct.

    - Click **Next**.
   The export file is imported.

    ![Click Import](images/import1.png " ")

3. To install the export file, click **Next**.

    ![Click Import](images/import.png " ")

4. Click **Install Application**.

    ![Click Import](images/install-app2.png " ")

5. Install Supporting Objects - This option only appears if the  Export includes supporting objects.

   To continue and install supporting objects:

     - **Install Supporting Objects**: ON

     - Click **Next**.

    ![Click Import](images/install-app1.png " ")

6. Click **Install**.

    ![Click Import](images/install-app.png " ")

   The export is installed.

7. Click **Edit Application**.

   ![Click Import](images/edit-app.png " ")

## Task 2: Change the Authentication Type in Social Media Application

The Social Media application is configured with a custom Security Authentication scheme. In this lab, you change the Authentication Type to Oracle APEX Accounts.

1. On the Workspace home page, click the **App Builder** icon. Select the Social Media application. On the Application home page, click **Shared Components**. The Shared Components page appears.

   ![Click Import](images/shared-comp.png " ")

2. Under Security, select **Authentication Schemes**. The Authentication Schemes page appears.

   ![Click Import](images/sc-authentication.png " ")

3. To create a new authentication scheme, click **Create**.

   ![Click Import](images/create-button.png " ")

4. Specify how the scheme should be created. In this case, select **Based on a pre-configured scheme from the gallery**.

   ![Click Import](images/create-authentication-scheme.png " ")

5. Specify a **Name** for Authentication Scheme.  For Scheme Type, select **Oracle APEX Account**.

   ![Click Import](images/oracle-apex-accounts1.png " ")

6. Click **Create Authentication Scheme**.


## Task 3: Add a Column to the Table using Object Browser

To collect the output generated by OCI AI Vision, you add a new column in SM\_POSTS Table. This addition enables you to store and retrieve the relevant information seamlessly.

To Add a new column to the SM\_POSTS Table:

1. Navigate to Object Browser. In the Object Tree, expand Tables and select **SM_POSTS** table.

    ![Click Import](images/add-column.png " ")

2. On the columns tab, Click **Add Column** under SM\_POSTS Table.


3. Configure the Add Column attributes. At a minimum, enter a column name and select a type. Depending upon the column type, specify whether the column requires precision, scale, a default value, or is nullable. For more details on an attribute, see field-level Help.

   Enter the following and click **Apply**.
      - **Column**: AI_OUTPUT
      - **Data Type**: VARCHAR2
      - **Length**: 1000

   ![Click Import](images/ai-output-column.png " ")

## Summary

You now know how to import the Oracle APEX application, change the authentication type, and add a new column.

You may now **proceed to the next lab**.   

## Acknowledgments

- **Author** - Roopesh Thokala, Senior Product Manager
- **Co-Author** - Ankita Beri, Product Manager
- **Last Updated By/Date** - Ankita Beri, Product Manager, August 2023   
