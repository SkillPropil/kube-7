# kube-7
## Задание 1
Файлы: [deployment](deployment.yaml) [pv-pvc](pv-pvc.yaml)  
После удаления deployment файл остался. Задание делал вчера, поэтому формулировка может быть немного неправильная. Файл остается потому что PV статически привязан к директории ноды.  
После удаления PV файл остался, так как директория /tmp/shared - директория ноды.  

<img width="797" alt="Снимок экрана 2024-09-27 в 00 03 31" src="https://github.com/user-attachments/assets/17e1a488-1f2d-46e2-b835-7b16e916b885">

## Задание 2
Файлы: [multitool](multitool-deployment.yaml) [nfs-pv](nfc-pv.yaml) [nfs-pvc](nfc-pvc.yaml)  
Данное задание делал уже сегодня, получилось далеекоооо не с первого раза, но все же смог:)  
В общем установил nfs-server на свою Centos9, расшарил папку /srv/nfsshare и подключил ее к поду мультитула. Из пода сделал туда  

```
echo "что-то" > lol.txt
```

Данная инфа записалась в файл и он даже остался на файловой системе ноды. Счастью не было предела:) Скрин ниже  
Препродам респект!  

<img width="799" alt="Снимок экрана 2024-09-27 в 21 41 55" src="https://github.com/user-attachments/assets/48baf46c-ac31-4e8b-8269-39ab7e80a2aa">
