# Copilot instructions for NetApp Replication documentation

## Repository overview

**Product:** NetApp Replication

NetApp Replication lets users copy data between ONTAP systems, Cloud Volumes ONTAP, and Amazon FSx for ONTAP for disaster recovery, backup, long-term retention, and data mobility. It uses SnapMirror and SnapVault technologies to keep destination volumes synchronized with a source volume. The product also helps users manage replication relationships, schedules, and transfer rates.

## Repository structure

* `_include` - Reusable text blocks referenced in .adoc files in the root. 
* `media` - Images and diagrams that are elements of articles in the root directory. This includes .png and source files. 
* `_whatsnew` - Release notes in .adoc form that are aggregated in the whats-new.adoc file.

## Product-specific context

- **NetApp Console:** The central management interface used to access and use NetApp Replication.
- **Console agent:** The cloud-deployed connector used to connect the Console to your storage systems and data services.
- **ONTAP cluster:** An ONTAP storage system, either on premises or in the cloud, that can participate in replication relationships.
- **Replication relationship:** The connection between the source and destination volumes that keeps data synchronized.
- **Replication policy:** The rule set that controls how data is copied, including SnapMirror and SnapVault behavior.
- **Schedule:** The timing for when replication transfers run, whether one time or on a recurrence.
- **Simple, fanout, and cascade configurations:** The supported protection patterns for one-to-one, one-to-many, and chained replication.

## Typical user workflows

- **Configure replication:** Set up a single or scheduled transfer when you need to move data; this can be a one-off event or a recurring event. This involves selecting the source and destination volumes, choosing a SnapMirror replication policy to meet the protection goal, and setting the transfer rate so that replication doesn't degrade other workload performance.
- **Manage existing relationships**: Check status, break or resync a relationship, reverse replication after failover, or update the schedule or transfer rate.