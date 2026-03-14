### How to push best practice?
1. **⚠️ jangan langsung push ke main kek gini❗:**

      ```
      git add .
      git commit -m "update"
      git push -u origin main
      ```
      Atau bahkan kek gini
      ```
      git push --force origin main
      ```

2. **✅ lakukan push dengan cara membuat branch baru dulu:
Pindah branch dan push dari branch ke dua**
      ```
      git branch risky
      git checkout risky
      git add .
      git commit -m "feat: perubahan apa"
      git push -u origin risky
      ```
      contoh
      <div style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; align-items: center;" align="center">
        <img width="400" alt="Image" src="https://github.com/user-attachments/assets/c9e973d7-5afb-41bb-8b36-6cd37c7817e3" align="center" /></div>
      <br>

      #### lebih best practices

      ```
      git git checkout -b feat/admin-dashboard
      git add .
      git commit -m "feat: perubahan apa"
      git push -u origin feat/admin-dashboard
      ```

      lalu lakukan Pull request untuk review, kunjungi link yang di berikan ketika push.
      contoh
        <div style="display: flex; flex-wrap: wrap;justify-content: center; align-items: center;" align="center">
          <img width="400" align="center" alt="Image" src="https://github.com/user-attachments/assets/25a5756c-909f-4986-8795-d8d3390fba44" />
      </div>
      <br>
        <div style="display: flex; flex-wrap: wrap;justify-content: center; align-items: center;" align="center">
          <img width="400" alt="Image" src="https://github.com/user-attachments/assets/e9e1cdc1-e8b9-4b1d-a7a5-d95c3098fc96" />
      </div>

      Create Pull request tapi jangan di merge. biar di partner melakukan review atau sesuai kesepakatan team.

3. Kalo udah di merge oleh partner atau diri sendiri, kembali ke vscode dan pull.
    ```
    git checkout main
    git pull
    ```
    nanti kalau mau buat fitur lagi, kembali ke awal dari checkout dulu ke branch lain.


### Resources
- https://youtu.be/BJu1Qcul7ig?si=AdVJjqjEVmeeNUcP
- https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
- https://learngitbranching.js.org/
- https://github.com/risky037/SISTA/issues/5
- https://www.conventionalcommits.org/en/v1.0.0/
- https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13