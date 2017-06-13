# abcdsh

The command control for the pods (bunch of sh's)  for the `Onboard Cloud` [project](https://github.com/megamsys/abcd)

## Usage

## ONE : Connect Node

1. To connect a host ip 127.0.0.1 to master using `default:` hypervisor kvm.

```
$ /var/lib/megam/abcdsh/one/connect-node.sh --hostip 127.0.0.1

```

2. To connect a host with ip 127.0.0.1 to master using hypervisor `xen`

```
$ /var/lib/megam/abcdsh/one/connect-node.sh --hostip 127.0.0.1 --hypervisor xen

```

## ONE : Create Storage

1. To create a fs datastore in opennebula master

```
$ /var/lib/megam/abcdsh/one/connect-storage.sh --nodeip 127.0.0.1 --fs fs
```

2. To create a NFS  datastore in opennebula master

```
$ /var/lib/megam/abcdsh/one/connect-storage.sh --nodeip 127.0.0.1  --fs nfs
```

3. To create a LVM  datastore in opennebula master  

```
$ /var/lib/megam/abcdsh/one/connect-storage.sh --nodeip 127.0.0.1  --fs lvm  
```
4. To create a CEPH  datastore to opennebula master

For ceph datastore add extra parameter `--secret f6f03141-2666` is required.

```
$ /var/lib/megam/abcdsh/one/connect-storage.sh --nodeip 127.0.0.1  --fs ceph --secret f6f03141-2666

```
