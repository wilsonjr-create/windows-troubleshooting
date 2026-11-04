# LAB-001 — Windows Performance Diagnostics

**Author**  Wilson Jr  
**Category**  Windows Troubleshooting / IT Support  
**Lab Type**  Personal Computer Performance Assessment  
**Status**  Initial Assessment Completed  
**Date**  04 November 2026

---

## 1. Objective

Evaluate the baseline performance of a Windows computer during an idle-state observation, focusing on CPU, memory, and disk utilisation.

## 2. Tools Used

- Windows Task Manager
- Performance tab

## 3. Diagnostic Procedure

1. Opened Windows Task Manager using `Ctrl + Shift + Esc`.
2. Navigated to the Performance tab.
3. Observed system resource utilisation during an idle-state assessment.
4. Recorded CPU, memory, and disk usage percentages.
5. Reviewed the readings for potential resource bottlenecks.

## 4. Results

| Component | Observed Usage | Assessment |
|---|---:|---|
| CPU | 5% | Low utilisation |
| Memory (RAM) | 60% | Moderate utilisation |
| Disk | 0% | No significant activity at the measurement point |

## 5. Technical Analysis

**CPU — 5%**

CPU utilisation was low during the observation. This reading does not suggest a CPU bottleneck at the time of measurement.

**Memory — 60%**

Memory utilisation was moderate. Further investigation would be required to determine whether background processes, startup applications, or available physical memory could affect system responsiveness.

**Disk — 0%**

No significant disk activity was observed at the measurement point. This reading does not indicate a disk utilisation bottleneck.

## 6. Preliminary Conclusion

The observed resource utilisation does not provide sufficient evidence of an active performance bottleneck.

No confirmed hardware or software fault was identified from these measurements alone.

Additional monitoring under normal workloads would be necessary to evaluate performance issues more thoroughly.

## 7. Recommended Follow-Up

- Review memory consumption by process.
- Identify unnecessary startup applications.
- Check system uptime and available memory.
- Monitor CPU, RAM, and disk usage under a normal workload.
- Review Windows Reliability Monitor if instability is reported.

## 8. Skills Demonstrated

- Windows Task Manager navigation
- Basic performance monitoring
- Resource utilisation analysis
- Technical documentation
- Structured IT troubleshooting
 
 ## 9. Follow-Up Assessment — Active Workload

### 9.1 Objective

Analyse Windows resource utilisation during normal multitasking and identify the applications consuming the most system memory.

### 9.2 Tools Used

- Windows Task Manager
- Processes tab
- Memory usage sorting

### 9.3 System Resource Utilisation

The second assessment was performed while multiple applications were running.

| Resource | Observed Usage |
|---|---:|
| CPU | 18% |
| Memory (RAM) | 68% |
| Disk | 0% |
| Network | 1% |

### 9.4 Highest Memory Consumers

The following applications were identified as the largest visible memory consumers.

| Application | Memory Usage |
|---|---:|
| Google Chrome (18 processes) | 2,949.3 MB |
| Discord (6 processes) | 357.2 MB |
| FACEIT (17 processes) | 337.0 MB |
| Spotify (12 processes) | 267.8 MB |
| EA | 135.0 MB |

### 9.5 Technical Findings

Google Chrome was the largest visible memory consumer, using approximately 2.95 GB of RAM across 18 processes.

Total system memory utilisation reached 68% while multiple applications were running.

CPU utilisation was 18%, and disk activity was minimal at the time of observation.

The results indicate that active applications contributed to overall memory consumption.

However, these measurements alone do not establish a hardware fault, memory leak, or operating system malfunction.

### 9.6 Troubleshooting Actions

1. Opened Windows Task Manager.
2. Selected the Processes tab.
3. Sorted applications by memory consumption.
4. Identified the highest memory-consuming applications.
5. Recorded resource utilisation and process information.
6. Selected Google Chrome for a follow-up memory comparison.

### 9.7 Preliminary Assessment

The system showed moderate-to-high memory utilisation during normal multitasking.

Google Chrome was identified as the primary visible memory consumer.

A follow-up test was planned to evaluate the impact of closing the browser on total system memory utilisation.

**Assessment Status:** Completed — Follow-up testing documented in Section 10.
---

**Portfolio:** Windows Troubleshooting & IT Support  
**Prepared by:** Wilson Jr  
**Career Focus:** IT Support Technician | Technical Support | Service Desk

## 10. Controlled Memory Usage Comparison

### Objective

Evaluate the impact of Google Chrome on system memory utilisation by comparing RAM usage before and after closing the browser.

### Test Procedure

1. Recorded system memory utilisation with Google Chrome running.
2. Identified Chrome as the largest visible memory consumer in Windows Task Manager.
3. Closed Google Chrome.
4. Waited approximately one minute.
5. Recorded the updated memory utilisation.

### Test Results

| Measurement | RAM Usage |
|---|---:|
| Before closing Chrome | 68% |
| After closing Chrome | 38% |
| Observed difference | -30 percentage points |
| Relative reduction | Approximately 44.1% |

### Technical Analysis

Google Chrome was consuming approximately 2.95 GB of RAM across 18 processes during the initial active-workload observation.

After closing Chrome, total system memory utilisation decreased from 68% to 38%.

This result strongly suggests that Chrome and its associated processes contributed substantially to the observed memory consumption.

However, other background activity and Windows memory management may also have influenced the measurements.

The test does not establish that Chrome was malfunctioning or that the system had a memory leak.

### Final Assessment

**Finding:** Significant reduction in memory utilisation after closing Google Chrome.

**Likely contributing factor:** Browser-related memory consumption during normal multitasking.

**Hardware fault:** Not identified from the available measurements.

**Resolution:** Closing the browser reduced memory utilisation. No hardware repair or permanent system modification was required.

### Recommendations

- Monitor browser memory consumption when experiencing system slowdowns.
- Close unused tabs and applications when additional memory is needed.
- Use Chrome's built-in Task Manager to identify resource-intensive tabs or extensions.
- Review startup applications periodically.
- Investigate further only if performance symptoms persist.

### Skills Demonstrated

- Windows performance monitoring
- Process resource analysis
- Before-and-after troubleshooting
- Technical interpretation of diagnostic results
- Evidence-based IT support documentation

### Lab Conclusion

The investigation demonstrated how application workloads can influence Windows memory utilisation.

The controlled comparison showed a 30-percentage-point reduction in memory usage after closing Google Chrome.

The results support an application-related explanation for the observed memory consumption, without establishing a hardware defect.

**LAB-001 Status: Completed — Initial Performance Investigation.**
