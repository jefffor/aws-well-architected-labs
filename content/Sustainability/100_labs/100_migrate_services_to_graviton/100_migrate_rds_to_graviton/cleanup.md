---
title: "Clean Up"
date: 2020-11-18T09:16:09-04:00
chapter: false
weight: 8
pre: "<b>3 </b>"
---

- [ ] [Migration Methodologies]({{< ref "./1_migration_methodologies.md" >}})
- [ ] [Preparation]({{< ref "./2-1_preparation.md" >}})
- [ ] [Lab 1 - Change Database Instance Type]({{< ref "./2-2_change_instance_type_and_restart.md" >}})
- [ ] [Lab 2 - Promote Read Replica]({{< ref "./2-3_promote_read_replica.md" >}})
- [ ] [Lab 3 - Failover to Read Replica]({{< ref "./2-4_failover_to_read_replica.md" >}})
- [ ] [Lab 4 - Restore from snapshot]({{< ref "./2-5_restore_from_snapshot.md" >}})
- [x] [Cleanup]({{< ref "./cleanup.md" >}})


## In the RDS Console delete all the created databases

{{% notice note %}}
**NOTE:** Because these are lab databases we will delete all the databases with their associated backups and will not create a final snapshot. 
Normally it would be highly recommended to create a final snapshot.
{{% /notice %}}


### Delete the Lab 1 RDS MySQL database

![Delete MySQL](/Sustainability/100_migrate_rds_to_graviton/clean-up/clean-up_delete_mysql.png)

### Delete the Lab 2 X86 database

![Delete Postgres X86](/Sustainability/100_migrate_rds_to_graviton/clean-up/clean-up_delete_postgres.png)

### Delete the Lab 2 Graviton Database

![Delete Postgres Graviton](/Sustainability/100_migrate_rds_to_graviton/clean-up/clean-up_delete_pg_graviton.png)


### Delete the Lab 3 Aurora Postgres X86 database

![Delete Aurora X86](/Sustainability/100_migrate_rds_to_graviton/clean-up/clean-up_delete_aurora_x86.png)

### Delete the Lab 3 Aurora Graviton database

![Delete Aurora Graviton](/Sustainability/100_migrate_rds_to_graviton/clean-up/clean-up_delete_aurora_graviton.png)

### Delete the Lab 4 MariaDB Database

![Delete Aurora Graviton](/Sustainability/100_migrate_rds_to_graviton/clean-up/clean-up_delete_mariadb.png)

If you took any manual snapshots, they should also be deleted.

{{< prev_next_button link_prev_url="../2-5_restore_from_snapshot" final_step="true" />}}