# Custom Commands

This readme details how to create custom DataMiner bot commands using Automation scripts.

## Table of Contents

- [Prerequisites](#prerequisites)
  - [Development](#Development)
    - [DataMiner Integration Studio Visual Studio Extension](#dataminer-integration-studio-visual-studio-extension)
  - [Usage](#Usage)
    - [General](#general)
    - [Microsoft Teams](#microsoft-teams)
- [Examples](#examples)
  - [General](#general-1)
  - [Microsoft Teams](#microsoft-teams-1)
    * [Getting Started](#getting-started)
    * [Output an Adaptive Card](#output-an-adaptive-card)
    * [Output Key-Values](#output-key-values)
    * [Output JSON](#output-json)
    * [Input Parameter](#input-parameter)
- [Help](#help)
- [Contact](#contact)
- [Version History](#version-history)
- [License](#license)

## Prerequisites

### Development

#### DataMiner Integration Studio Visual Studio Extension

The DataMiner Integration Studio Visual Studio extension (also referred to as DIS) can be used for development of Automation scripts. You can also use DIS to deploy Automation scripts directly from your development environment to your DataMiner Systems.

See [Installing DataMiner Integration Studio](https://aka.dataminer.services/DisInstallation).

> ℹ️
> We recommend that you always use the latest version of the DataMiner Integration Studio Visual Studio extension.

### Usage

#### General

- The DataMiner System must be cloud-connected. See [Connecting your DataMiner System to the cloud](https://docs.dataminer.services/user-guide/Cloud_Platform/AboutCloudPlatform/Connecting_your_DataMiner_System_to_the_cloud.html).

- The CoreGateway module must be updated to at least version 2.11.0 (which is available since [Cloud Pack 2.8.0](https://community.dataminer.services/downloads/)). See [Upgrading nodes to the latest DxM versions](https://docs.dataminer.services/user-guide/Cloud_Platform/CloudAdminApp/Managing_cloud-connected_nodes.html).

- The FieldControl module must be updated to at least version 2.8.1 (which is available since [Cloud Pack 2.8.0](https://community.dataminer.services/downloads/)). See [Upgrading nodes to the latest DxM versions](https://docs.dataminer.services/user-guide/Cloud_Platform/CloudAdminApp/Managing_cloud-connected_nodes.html).

#### Microsoft Teams

- The [DataMiner bot](https://teams.microsoft.com/l/app/9a09d087-5d07-4481-b34f-cd053eab7925) must be allowed in your [Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/manage-apps).

- The [DataMiner bot](https://teams.microsoft.com/l/app/9a09d087-5d07-4481-b34f-cd053eab7925) must be installed in your team or chat. See [Installing the DataMiner Teams bot](https://docs.dataminer.services/user-guide/Cloud_Platform/TeamsBot/DataMiner_Teams_bot.html#dataminer-teams-bot-installation).

- [Start a conversation with the DataMiner bot](https://docs.dataminer.services/user-guide/Cloud_Platform/TeamsBot/DataMiner_Teams_bot.html#starting-a-conversation-with-the-teams-bot) by logging in and setting your active DataMiner System. When you execute your first (custom) command to the active DMS, the DataMiner bot will ask you to link your DCP account to your DataMiner account if this has not been done yet.

- Only Automation scripts that are present in a (sub)folder with the name '*bot*' will be recognized as custom commands by the DataMiner bot. The examples below are automatically placed in such a folder.

## Examples

### General

- The code for these Automation scripts can be found in [the CustomCommandExamples folder](). Note that these examples are kept very simple, without user input, and they only demonstrate how to form different types of output to be displayed by the DataMiner bot. For more information about what Automation scripts can do, see [Automation](https://docs.dataminer.services/user-guide/Advanced_Modules/Automation/automation.html).

### Microsoft Teams

#### Getting Started

1. [Deploy the latest version of the Custom Commands Examples package via the Catalog](https://catalog.dataminer.services/catalog/5212) or [download the package as a ZIP](https://github.com/SkylineCommunications/ChatOps-Extensions/files/9673583/DcpCustomCommandExamples.1.0.0.X_B5.zip), unzip it, and [deploy it to your DataMiner System locally](https://aka.dataminer.services/installing-application-packages). Installing this package will add the custom command Automation scripts for Microsoft Teams in the Automation module.

   > :warning:
   > Installing this DMAPP will overwrite any Automation scripts with identical names.

#### Output an Adaptive Card

1. In Teams, execute the command '*run Adaptive Card Output Example*' and click the '*Run*' button in the response.

2. The custom command will be executed and the Adaptive Card example should be displayed as the response. <details><summary>`show demo`</summary>![Gif-OutputAnAdaptiveCard](https://user-images.githubusercontent.com/33500507/192817296-cd05a0cb-2267-4639-8d21-32b54bb347cd.gif)</details>

#### Output Key-Values

1. In Teams, execute the command '*run Key Value Output Example*' and click the '*Run*' button in the response.

2. The custom command will be executed and the Key Value examples should be displayed as the response. <details><summary>`show demo`</summary>![Gif-OutputKeyValues](https://user-images.githubusercontent.com/33500507/192817311-75f6e7c0-0c91-45e1-9f58-30783fb67ddf.gif)</details>

#### Output JSON

1. In Teams, execute the command '*run JSON Output Example*' and click the '*Run*' button in the response.

2. The custom command will be executed and the JSON example should be displayed as the response. <details><summary>`show demo`</summary>![Gif-OutputJson](https://user-images.githubusercontent.com/33500507/192817316-fc4de34d-a34e-42cd-a5fa-e8e99b363c2d.gif)</details>

#### Input Parameter

1. In Teams, execute the command '*run Input Parameter Example*'.

2. When you are asked to provide the input configured in the Automation script, fill in any value and click the '*Run*' button.

   The custom command will be executed, and the provided input value should be displayed as the response. <details><summary>`show demo`</summary>![Gif-InputParameter](https://user-images.githubusercontent.com/33500507/233356486-bc64d385-997e-4b1b-8466-e26c801a7e4d.gif)</details>

## Help

[Skyline Communications: Support](https://aka.dataminer.services/tech-support)

## Contact

[Skyline Communications: Contact](https://aka.dataminer.services/contact)

## Version History

[Releases](https://github.com/SkylineCommunications/ChatOpts-Extensions/releases)

## License

This project is licensed under the [MIT License](https://github.com/SkylineCommunications/ChatOps-Extensions/blob/main/LICENSE) – see the file for details.
