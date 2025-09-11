---
title: "Millennia Chat"
---

# Millennia Chat

> **Connection (Internet):** `aim.millennia.chat`  
> **Connection (Show DSL):** `TBD`

**Protocol:** AIM (OSCAR) — **Default port: `5190`**

---

## Step‑by‑step: Setting up the classic Windows AIM client

1. **Install AIM** (versions **2.x–5.x** are supported with Millennia Chat).
   - If you are running Windows 10/11 you may need to run the installer in compatibility mode for older Windows (e.g. Windows XP SP3).
2. **Open AIM** but do not sign on yet.
3. Click the **Setup** (yellow wrench) button, then **Connection**.
   
   ![Windows AIM Setup Screen Placeholder](images/windows-aim-setup.png)

4. Replace the **Host** with `aim.millennia.chat` and set **Port** to `5190`.
   
   ![Windows AIM Connection Settings Placeholder](images/windows-aim-connection.png)

5. Make sure **Connect using proxy** is **unchecked**.
6. Click **OK** → **OK**.
7. Enter your screen name and password and click **Sign On**.

---

## Step‑by‑step: Connecting with a classic Macintosh AIM client (Mac OS 7, 8, 9)

Classic AIM clients for Mac OS 7/8/9 do not provide an interface to change the server host. You must use **ResEdit** to modify the application resources:

1. **Download and install ResEdit** from Apple’s archived tools.
2. Make a **backup copy** of your AIM application.
3. Open the AIM application with ResEdit.
   
   ![ResEdit Application Placeholder](images/resedit-open.png)

4. Locate the **STR# resource** that contains server addresses.
   - This is usually labeled with IDs corresponding to connection hosts.
   
   ![ResEdit STR Resource Placeholder](images/resedit-str-resource.png)

5. Find the default server entry (commonly something like `login.oscar.aol.com`).
6. Replace the server string with: `aim.millennia.chat`.
   
   ![ResEdit Edit String Placeholder](images/resedit-edit-string.png)

7. Save the changes and close ResEdit.
8. Launch AIM and sign on with your Millennia Chat screen name and password.

**Note:** Do not change any other strings or resources to avoid corrupting the application.

---

## Attribution

- This server and the software powering it are built with **Retro AIM Server** — many thanks to the project and contributors: https://github.com/mk6i/retro-aim-server
- The **Millennia Chat Welcome Bot**, which sends new users a greeting with server rules and a link to the public chatroom, is powered by scripts adapted from: https://github.com/jgknight/ras-scripts/tree/main/signon_monitor
