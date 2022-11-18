---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Uninstall the Workfront for Adobe Experience Manager enhanced connector
description: You must uninstall the Workfront with Adobe Experience Manager enhanced connector to the latest native integration connecting Workfront and Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
---
# Uninstall the Workfront with Adobe Experience Manager enhanced connector

You must uninstall the Workfront with Adobe Experience Manager enhanced connector to the latest native integration connecting Workfront and Adobe Experience Manager Assets as a Cloud Service.

## Prerequisites 

* (Optional) If necessary, revert any changes that were made to the Workfront firewall configuration and AEM dispatcher settings.

## Uninstall the enhanced connector

1.  Access and clone your AEM as a Cloud Service repository from Cloud Manager.

1. Open your cloned git repository in the IDE of your choice.

1. Checkout the branch where the enhanced connector is installed.

1. Navigate to the following path and remove the enhanced connector zip file: 

    `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Remove the following dependency from the pom.xml file of the project's root.

   ``` 
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Please ensure the version referenced in above code block, i.e 1.8.0, reflects the version that is being uninstalled from the code.

1. Remove the following dependency from the pom.xml file of the project's submodule named **all**.

    ```
    <!-- Workfront Tools -->
    <embedded>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <target>/apps/<path-to-project-install-folder>/install</target>
    </embedded>
    ```
1. Remove the following embedded from the pom.xml file of  the project's submodule named all.

    ```
    <!-- Workfront Tools -->
    <embedded>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <target>/apps/<path-to-project-install-folder>/install</target>
    </embedded>
    ```

1. (Conditional) Remove the repository configuration from the pom.xml file of the project's root.


    ```
    <repository>
        <id>hoodoo-maven</id>
        <name>Hoodoo Repository</name>
        <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
    </repository>
    ```

1. (Conditional) Remove the server configuration from the settings.xml, present in the following path ./cloudmanager/maven/settings.xml in the project root.'

    ```

            <server>
            <id>hoodoo-maven</id>
            <configuration>
                <httpHeaders>
                    <property>
                        <name>Deploy-Token</name>
                        <value>*********************</value>
                    </property>
                </httpHeaders>
            </configuration>
        </server>
    ```

1. Commit the changes, and push the code to the Cloud Manager repository

1. Run the Cloud Manager pipeline to deploy the changes on your Cloud Services instance
