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

<h2>🌍 Environments and Technologies Used</h2>

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
- This is the Admin Login URL http://localhost/osTicket/scp/login.php
- And this is the User URL http://localhost/osTicket
  
<details>
  <summary>1️⃣ 👤 Configure an Admin Role</summary>

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
  <summary>2️⃣ 🛠️ Create a SysAdmin Department</summary>

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
  <summary>3️⃣ 👥 Configure a Team</summary>

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
  <summary>Configure Roles</summary>
</details>

<details>
  <summary>Configure Roles</summary>
</details>

<details>
  <summary>Configure Roles</summary>
</details>

<details>
  <summary>Configure Roles</summary>
</details>


<!-- 1️⃣ 2️⃣ 3️⃣ 4️⃣ 5️⃣ 6️⃣ 7️⃣ 8️⃣ 9️⃣ -->
