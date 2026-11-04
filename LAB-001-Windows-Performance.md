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

---

**Portfolio:** Windows Troubleshooting & IT Support  
**Prepared by:** Wilson Jr  
**Career Focus:** IT Support Technician | Technical Support | Service Desk
