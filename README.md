# Ansible Git Branching Task

## Task Description

Your task is to create **four branches** in your Git repository:

1. **`ansible-all`**  
   - This branch should contain **all Ansible roles**.  
   - Exclude the **host inventory** from the repository using `.gitignore`.

2. **`ansible-web`**  
   - This branch should include only the roles:  
     - `zabbix-agent`  
     - `redis`

3. **`ansible-user`**  
   - This branch should contain only the **user role**.  
   - **Do not include** the **public SSH key (`pub` file)** in the repository.

4. **`ansible-merge`**  
   - This branch should be created by merging:  
     - `ansible-web`  
     - `ansible-user`  

## Steps to Complete

1. **Create the branches:**
   ```sh
   git checkout -b ansible-all
   git checkout -b ansible-web
   git checkout -b ansible-user
   git checkout -b ansible-merge

