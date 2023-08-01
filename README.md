# Public Scripts
---
```bash
curl -sSL https://raw.githubusercontent.com/GaurAfro/Public_Script/blob/23b9956001dea922ddff794ced70e6e88fbed77c/setup_git.sh | bash
```
---

### **Using the `add_current_user_to_sudoers.sh` Script with `curl`**

This guide will walk you through the process of executing the `add_current_user_to_sudoers.sh` script using `curl`.

#### **Instructions**:

1. **Switch to the Superuser**: Before running the script, ensure you are the superuser (root).
   ```bash
   su
   ```
2. **Install `curl`**: If it's not already installed, you can get it with:
   ```bash
   apt install curl
   ```
3. **Execute the Script**: Now, execute the following command:
   ```bash
   curl -sSL https://raw.githubusercontent.com/GaurAfro/Public_Script/blob/d0acc3dae85637ba33969befd6027da6160294b8/add_current_user_to_sudoers.sh | bash
   ```

3. **Script Execution**: The script will run and automatically configure the necessary settings to grant sudo privileges to the current user.

4. **Verification**: To verify, exit from the superuser mode:
   ```bash
   exit
   ```
   Then, try a sudo command to ensure the current user has been added to the `sudoers`:
   ```bash
   sudo apt update && sudo apt upgrade -y
   ```

5. **Completion**: If the `sudo` command runs without any permission issues, the script has successfully added the user to the `sudoers`.

#### **Safety Reminder**:
Always ensure you trust the source of scripts you're fetching and executing directly from the web. It's a good practice to review the content of scripts before running them, especially as a superuser.

---
