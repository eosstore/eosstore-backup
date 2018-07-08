# eosstore-backup
mainnet data backup

In order to ensure the security of the main network, we made regular backup of the data.We backup data once a day,and include blocks and state.

We can get the data from [EOSSTORE-backup-address](https://s3-ap-northeast-1.amazonaws.com/eosstorebp/index.html)
OS:Ubuntu16.04

Put the data at your bp's data-dir

1.Get lastly data with 
```
wget https://s3-ap-northeast-1.amazonaws.com/eosstorebp/xxx.tar.gz
```

2.then tar the xxx.tar.gz

```
tar -zxvf xxx.tar.gz
```

3.we can see two folder.
```
root@eos-test-01:/data/eos-data# ll
total 20
drwxr-xr-x 5 1001 1001 4096 Jul  2 09:59 ./
drwxr-xr-x 4 root root 4096 Jul  2 10:08 ../
drwxrwxr-x 3 1001 1001 4096 Jun 25 13:57 blocks/
drwxrwxr-x 2 1001 1001 4096 Jul  2 10:08 state/
root@eos-test-01:/data/eos-data# ls
```

4.start your nodeos
