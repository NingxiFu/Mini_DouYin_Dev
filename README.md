# Mini_DouYin_Dev
### Developing...Saved here for solid synchronization and my own readability.

#### user:
```shell
cd cmd/user
```
```shell
sh output/bootstrap.sh
```

#### api:
```shell
cd cmd/api
```
```shell
go run .
```

#### etcd:
```shell
cd etcd
```
```shell
etcd \
--name=default \
--data-dir=default.etcd \
--listen-peer-urls=http://localhost:2380 \
--listen-client-urls=http://localhost:2379 \
--initial-advertise-peer-urls=http://localhost:2380 \
--initial-cluster=default=http://localhost:2380 \
--initial-cluster-state=new \
--initial-cluster-token=etcd-cluster \
--advertise-client-urls=http://localhost:2379 \
--logger=capnslog
```

```shell
git add .
```
```shell
git commit -m ""
```
```shell
git push origin main
```

