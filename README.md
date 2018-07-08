# eosstore-backup
mainnet data backup

In order to ensure the security of the main network, we made regular backup of the data.We backup data once a day,and include blocks and state.

You can see the data at [EOSSTORE-backup-address](https://s3-ap-northeast-1.amazonaws.com/eosstorebp/index.html)

Get data with 
```
wget https://s3-ap-northeast-1.amazonaws.com/eosstorebp/xxx.tar.gz
```

```
root@eos-test-01:/data/eos-data# ll
total 20
drwxr-xr-x 5 1001 1001 4096 Jul  2 09:59 ./
drwxr-xr-x 4 root root 4096 Jul  2 10:08 ../
drwxrwxr-x 3 1001 1001 4096 Jun 25 13:57 blocks/
drwxrwxr-x 2 1001 1001 4096 Jul  2 10:08 state/
root@eos-test-01:/data/eos-data# ls
```
