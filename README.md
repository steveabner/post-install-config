<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project focuses on configuring osTicket by setting up multiple agents, departments, roles, and permissions. Additionally, I will configure SLAs, help topics, and users..<br/>
<br/>

This project is a continuation of the [osTicket: Prerequisites and Installation](https://github.com/steveabner/osticket-prereqs) project.
<br/>

<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>🌍 Environments and Technologies Used 🌍</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket
- Internet Information Services (IIS)
  
<h2>🖥️ Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>🛠️ Post-Install Configuration Objectives</h2>

- Configuring roles, departments, and teams
- Configuring agents and users
- Configuring SLAs
- Configuring Help Topics

<h2>⚙️ Configuration Steps</h2>

- In this section, I will be using the Admin/Analyst Login Page and the End Users osTicket URL.
- Admin Login URL - http://localhost/osTicket/scp/login.php
- User URL - http://localhost/osTicket

`⬇️ Click to Expand ⬇️`
<details>
  <summary> 👤 Configure an Admin Role 👤</summary>

- Log into osTicket through the admin page.

  ![2025-01-06 22_03_53-Window](https://github.com/user-attachments/assets/3059ac7a-d200-40b3-bc4d-cae5fb67b6ce)

- On the Admin Panel, click `Agents`

  ![2025-01-06 22_01_32-Window](https://github.com/user-attachments/assets/8dedae53-4c86-4455-802c-841c41142c42)

- Then click `Roles`

  ![2025-01-06 22_02_13-Window](https://github.com/user-attachments/assets/48b4aae0-0ec6-4ae5-b7a0-d8f9560cac86)

- On the roles panel, click `Add New Roles`

  ![2025-01-06 22_02_39-Window](https://github.com/user-attachments/assets/39428a37-4eaf-4a16-ba39-68cc93b4fa28)

- I'll name the role `Admin`, then click `Permissions`.

  ![2025-01-06 22_08_24-Window](https://github.com/user-attachments/assets/8bab2069-8907-4652-968d-678c3476cebb)

- On the Permissions tab, I will check every permission in the `Tickets`, `Tasks`, and `Knowledgebase` tabs. Then click `Add Role`.

  ![2025-01-06 22_08_48-Window](https://github.com/user-attachments/assets/da84e14d-2d43-4d20-9cde-3850622247c3)
  ![2025-01-06 22_09_05-Window](https://github.com/user-attachments/assets/25331469-7de7-4cd6-aec4-1c56a883e384)
  ![2025-01-06 22_09_17-Window](https://github.com/user-attachments/assets/ad9b7fdc-7299-42df-90cb-df0516afa1a8)

- I now have an Admin Role.

  ![2025-01-06 22_15_18-Window](https://github.com/user-attachments/assets/bc246678-2cd4-45d0-a51c-a6c6e9700f7a)

</details>

<details>
  <summary> 🛠️ Create a SysAdmin Department 🛠️</summary>

- On the admin panel, hover over `Agents`, then click `Departments` 

  ![2025-01-06 22_20_54-Window](https://github.com/user-attachments/assets/45778ea4-b6b8-4bcd-ae16-f4de879a8a44)

- On the Departments page, click `Add New Department`

  ![2025-01-06 22_22_13-Window](https://github.com/user-attachments/assets/17f0b4b4-3bf2-490d-a168-505f3ea13919)

- I'll name the department `SysAdmin`, then click `Create Dept`. Leave other settings as `Default` for now.

  ![2025-01-06 22_25_34-Window](https://github.com/user-attachments/assets/158dc599-b56b-4f5c-bc53-0e7f6a38676f)

- I now have a SysAdmin department set up.

  ![2025-01-06 22_29_30-Window](https://github.com/user-attachments/assets/8558a2f6-cb68-4411-8573-cf7c8ac368dd)

</details>

<details>
  <summary> 🤝 Configure a Team 🤝</summary>

- On the Admin Panel, Hover over `Agents`, then click `Teams`

  ![2025-01-06 22_42_19-Window](https://github.com/user-attachments/assets/8c02e93f-6a05-4f9e-b99b-ce782429c91a)

- On the teams panel, click `Add New Team`

  ![2025-01-06 22_43_28-Window](https://github.com/user-attachments/assets/38499a6a-8659-4084-a508-a51ce9cde6e3)

- I'll name it `Online-Banking`, then click `Create Team`. I'll leave everything else as is. 

  ![2025-01-06 22_44_25-Window](https://github.com/user-attachments/assets/67a51df9-a191-4126-947e-675a3293c5ff)

- I now have a team called Online-Banking.

  ![2025-01-06 22_46_18-Window](https://github.com/user-attachments/assets/7dba1b7c-ed2e-4d9d-83f6-61dce706b528)

</details>

<details>
  <summary> 📝 Allow users to create tickets without an account 📝</summary>

- On the Admin Panel, hover over `Settings`, then click `Users`.

  ![2025-01-06 22_50_55-Window](https://github.com/user-attachments/assets/aa6892ff-7d8a-4405-92f5-d2419d36f7a9)

- On the user settings page, just make sure `Require registration and login to create tickets` is unchecked, then click `Save Changes`.

  ![2025-01-06 22_52_53-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/a62a537c-0b52-4df6-9e86-be388014b882)
  
</details>

<details>
  <summary> 👥 Create Agents (Workers) 👥</summary>

- On the Admin Panel, click `Agents`.

  ![2025-01-06 23_04_54-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/4c376fb6-9987-4563-b2fc-3a8c2f5bbb69)

- On the Agent page click `Add New Agent`.

  ![2025-01-06 23_06_15-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/ccf084ce-79a1-4685-ae04-0187ed0fe549)

- I'll name this Agent `John Smith`, input a fake email, set the username to `John`, then click `Set Password`.

  ![2025-01-06 23_14_15-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/a801a348-1eaf-4f3d-8e08-69c015d84e1f)

- On the `Set Agent Password` screen, uncheck `Send the agent a password reset email`, input a password, then uncheck `Require password change at next login`. Then click `Set`.

  ![2025-01-06 23_13_57-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/3cc60236-0b1d-4bc0-90de-f573141f907f)

- Next, I'll click the `Access` tab.

  ![2025-01-06 23_18_28-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/6b976992-7411-4e61-9617-d95161da959b)

- On the access tab, I'll set the department to `SysAdmin`, and give the `Admin` Role.

- Next, I'll click the `Teams` tab.

  ![2025-01-06 23_21_15-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/64526cf0-65a0-4ff2-b789-958b3313c1d0)

- On the teams tab, I'll select `Online-Banking`, and then click `Add`, and finally, click `Create`

  ![2025-01-06 23_22_55-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/eb7bcfd1-f7b3-4bfd-9a13-4424d3dc2a35)
  ![2025-01-06 23_23_52-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/f575c883-1070-4d8b-8626-b1117546b0ac)

- John has been created, Now I'll create one more Agent. On the Agents page, I'll click `Add New Agent`

  ![2025-01-06 23_36_14-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/d2cb0d79-3447-450e-b831-a6f4820d2989)

- I'll input the name `Jane Doe`, input an email, and set a password.

  ![2025-01-06 23_38_25-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/80de9c3f-e44f-4797-8731-87c281284f41)

- Next, I'll click `Access` 

  ![2025-01-06 23_38_25-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/a0de32f6-b53c-4a5e-99b8-f25ee896303b)

- On the Access tab, I'll select the `Support` department, set the role to `All Access`, then click `Create`

  ![2025-01-06 23_44_47-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/c19f08b8-b1ef-4002-b961-a630c7fbbb7c)

</details>

<details>
  <summary> 👥 Configure Users (Customers) 👥</summary>

- On the osTicket dashboard, I'll click `Agent Panel` at the top-right of the browser.

  ![2025-01-07 11_16_11-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/0840114c-f385-4cbc-a55c-6e157d1ae978)

- On the Agent Panel, I'll click `Users`

  ![2025-01-07 11_17_50-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/1ae3bedd-ff23-4bf1-aa97-26edb9d974b9)

- On the User page, click `Add User`

  ![2025-01-07 11_19_17-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/d7a2f801-fc63-43c2-9be7-eefb6a94388e)

- I'll input the name `Sarah`, an email, then click `Add User`

  ![2025-01-07 11_22_26-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/47ec41d9-419d-4946-9502-97206307859b)

- I'll do this once more, and create another User named `Karen`.

  ![2025-01-07 11_25_48-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/de209247-bdb3-40c4-913b-e42927f98a5f)

- Now I have two Users, `Sarah` and `Karen`.

  ![2025-01-07 11_26_09-48 211 167 121 - Remote Desktop Connection](https://github.com/user-attachments/assets/1d7c0a3c-6383-4bbb-81aa-a7ddd6c9cc28)

</details>

<details>
  <summary> 📜 Configure SLA 📜</summary>














</details>


<!-- 1️⃣ 2️⃣ 3️⃣ 4️⃣ 5️⃣ 6️⃣ 7️⃣ 8️⃣ 9️⃣ -->
