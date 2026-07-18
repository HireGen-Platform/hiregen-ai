# Quick Setup Guide - Platform & Security (Team 1)

Hey guys, yahan quick steps hain project setup karne ke liye taaki sab log shuru kar sakein.

## Requirements (Install kar lena):
- Node.js (LTS version download kar lo)
- Git (command line ya GitHub Desktop jo sahi lage)
- PostgreSQL (database ke liye)
- VS Code editor

## Steps to run:
1. Folder ke andar jaao:
   `cd platform-security`
2. Packages install karo:
   `npm install`  (agar error aaye powershell script block ka toh `npm.cmd install` chalana)
3. Server run karke check karo:
   `node src/server.js` (port 3000 par run hona chahiye)

## Folder layout kya hai:
- `routes/` -> endpoints definitions aur zod validations
- `controllers/` -> requests ko routes se services tak pass karna
- `services/` -> actual logic (like login verification, hashing passwords, generating tokens)
- `repositories/` -> direct raw SQL queries (no database queries in routes or services)
- `middleware/` -> JWT validation and role-based permissions (RBAC)
- `config/` -> db config variables

## Help:
Seekhne ke liye ChatGPT/Claude ki help le sakte ho (jaise zod validations ya fastify setup ke codes search kar lo). Kuch bhi block ho toh group par screenshot daal dena, discuss karke fix karenge.

*Archana: laptop issue solve hone tak aap login/auth ke logic, requirements list aur validation test cases hand-written design karengi, and pull requests review karengi on GitHub mobile.*
