# Implementing-wordpress-website-with-LVM-storage-management



sudo lvcreate -n db-lv -L 14G webdata-vg
sudo lvcreate -n logs-lv -L 14G webdata-vg

sudo mkfs -t ext4 /dev/webdata-vg/db-lv
sudo mkfs -t ext4 /dev/webdata-vg/logs-lv

sudo mount /dev/webdata-vg/db-lv /var/db

sudo rsync -av /home/recovery/logs. /var/log









