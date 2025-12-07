Business continuity ensures the organization can continue essential operations during a disruption.  
Resilience and redundancy reduce downtime, protect critical functions, and support fast recovery.  
Your exam will test your understanding of BCP vs DRP, key metrics such as RTO/RPO/MTTR/MTBF, and how redundancy mechanisms enable operational continuity.

---

## 12.1 Planning Frameworks (BCP, DRP, BIA)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Business Continuity Planning (BCP) | Ensures organizational operations continue during and after disruptions. | • Focus: business processes<br>• Includes people, facilities, tech<br>• Requires identifying critical functions | EisnerAmper continuing financial reporting even if office network fails. |
| ★ Disaster Recovery Planning (DRP) | Focuses on restoring IT systems, data, and infrastructure after an outage. | • Technical recovery plan<br>• Involves backup, failover, rebuild | Restoring access to Yardi or shared drives after a server outage. |
| ★ Business Impact Analysis (BIA) | Identifies mission-critical processes and the impact of downtime. | • Determines RTO/RPO<br>• Helps prioritize recovery strategy | Identifying which reporting workflows cannot be delayed. |
| Comparison | BCP = maintain operations; DRP = restore systems. | • BIA informs both BCP & DRP | Reporting deadlines prioritized during an outage based on BIA findings. |

---

## 12.2 Key Resilience Metrics (RTO, RPO, MTTR, MTBF)

| Metric | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|--------|----------------------|----------------------------------|--------------------|
| ★ Resilience Metrics | Measurements guiding recovery expectations and system reliability. | • Define downtime limits<br>• Define data loss tolerance | Used when planning backup frequency for client financial data. |
| RTO (Recovery Time Objective) | Maximum acceptable downtime for a system. | • Time-based<br>• “How long can we be down?” | Reporting system must be restored within a certain number of hours. |
| RPO (Recovery Point Objective) | Maximum acceptable amount of data loss measured in time. | • Backup frequency<br>• “How much data can we afford to lose?” | Backups of client schedules run nightly to minimize data loss. |
| MTTR (Mean Time to Recovery) | Average time to repair/restore a system. | • Focus: fix speed | IT restoring a shared drive after corruption. |
| MTBF (Mean Time Between Failures) | Average time a system runs without failing. | • Predicts reliability | Planning replacement of aging reporting servers. |
| Comparison | RTO = downtime; RPO = data loss; MTTR = repair time; MTBF = failure likelihood. | • Exam will test differences | Knowing reporting must resume quickly with minimal lost work. |

---

## 12.3 Resilience Mechanisms (Redundancy & Failover)

| Mechanism | Expanded Definition | Nested Key Points | Workplace Example |
|-----------|----------------------|--------------------|--------------------|
| ★ Redundancy | Duplicate systems or components to ensure continuity. | • Eliminates single points of failure<br>• Supports high availability | Backup servers storing accounting data for recovery. |
| Server Clustering | Multiple servers act as one for load balancing or failover. | • Active-active<br>• Active-passive | Reporting servers configured to failover automatically. |
| Storage Redundancy (RAID) | Protects against disk failure. | • RAID 1 = mirroring<br>• RAID 5 = parity<br>• RAID 10 = performance + redundancy | Protects reporting data on internal file storage. |
| Backups | Copies of data stored for restoration. | • Full, differential, incremental<br>• Offsite & cloud options | Backups of client folders used when a file is lost or corrupted. |
| High-Availability Architecture | Systems designed to stay online continuously. | • Load balancers<br>• Redundant network paths | Ensuring Yardi or financial portals remain accessible during outages. |

---

## 12.4 Continuity Challenges & Risks

| Challenge | Expanded Definition | Nested Key Points | Workplace Example |
|-----------|----------------------|--------------------|--------------------|
| Backup Gaps | Backups that are too infrequent or incomplete. | • Increases RPO<br>• More data lost in failure | Only nightly backups → entire day of financial changes lost if system fails. |
| Single Points of Failure | One component whose failure disrupts everything. | • Critical in OT & IT<br>• Must be eliminated | Overreliance on a single reporting system like Yardi. |
| Resource Constraints | Not enough staff or tech to recover quickly. | • Increases MTTR<br>• Impacts operations | IT slow to restore shared drives due to limited staffing. |

---

## 12.5 Study Focus Summary

| Exam Topic                        | Explanation                                            |
| --------------------------------- | ------------------------------------------------------ |
| BCP vs DRP                        | BCP = maintain operations; DRP = restore systems.      |
| RTO vs RPO                        | RTO = downtime allowed; RPO = data loss allowed.       |
| Redundancy Types                  | Clustering, RAID, backups, failover.                   |
| BIA Role                          | Determines critical functions and recovery priorities. |
| Avoiding Single Points of Failure | Essential for resilience.                              |