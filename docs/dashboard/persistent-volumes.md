---
id: persistent-volumes
title: 📦 Persistent Volumes
sidebar_position: 4
---

In **Persistent Volumes** section, you can see all the persistent volumes created across your cluster for your applications.

![Persistent Volume List](/assets/persistent-volumes.png)

### Create a Persistent Volume
1. **Local Volume**
   Local volume is a volume that is created on the local storage of the node. It is not shared across the cluster.

   - Click on `Add New` button.
   - ![Local Volume](/assets/create-local-volume.png)
   - Choose a unique name for the volume and can't contain spaces.
   - Choose type `Local`.
   - Click on `Register` button and the volume will be created.

2. **NFS Volume**
   You can create a NFS volume to share the volume across the cluster and also to keep your data more reliable.

   - Click on `Add New` button.
   - ![NFS Volume](/assets/create-nfs-volume.png)
   - Choose a unique name for the volume and can't contain spaces.
   - Choose type `NFS`.
   - Fillup NFS server details.
     > Note : Duly check the NFS server details before submitting. You can't change the NFS server details once the volume is created.
   - Click on `Register` button and the volume will be created.


### Delete a Persistent Volume
Just click on `Delete` button to delete a persistent volume.

### Analyze Size of Persistent Volume
You can click on `Fetch Size` button to fetch size of the persistent volume.

### Backup Volume
1. You can backup and take snapshot of the persistent volume by clicking on `Create Backup` button.
2. You can choose type of backup.
    - **Local** : The backup will be stored locally in the server itself.
    - **S3** : The backup will be stored in S3 bucket. You need to configure S3 beforehand to avail this feature.
      > You can open  swiftwave config by [`swiftwave config -e vim`](/docs/cli/config) command
3. Submit to create backup.
4. You can open the backup history by `Show Backups` button to see the status of the backup.

### Backup History
You can click on `Show Backups` button to see the backup history of the volume.

![Backup History](/assets/backup-history.png)

- You can check status of old backups.
- You can also download the backup file by clicking on `Download Backup` button.


### Restore Volume
1. You can upload a backup file to restore the volume by clicking on `Restore Now` button.
2. Upload the backup file.
3. Submit to restore the volume.
4. You can open the restore history by `Show Restores` button to see the status of the restore.

### Restore History
You can click on `Restore History` button to see the restore history of the volume.

![Restore History](/assets/restore-history.png)

- You can check status of all restores.