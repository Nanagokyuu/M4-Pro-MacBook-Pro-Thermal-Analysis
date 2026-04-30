This performance report outlines the thermal throttling behavior and stability of the **MacBook Pro (M4 Pro) 14”.** under various power and cooling configurations using the **3DMark Steel Nomad Light** stress test.

---

## 💻 System Specifications
*   **Device:** MacBook Pro (M4 Pro) 14”.
*   **CPU:** 14-Core
*   **GPU:** 20-Core
*   **Memory:** 48GB Unified Memory
*   **OS:** macOS 26.2
*   **Graphics API:** Metal

---

## 📈 Benchmark Results: Steel Nomad Light (Unlimited Stress Test)

### 1. Plugged In | High Power Mode | Default Fan Curve
This configuration represents the peak sustained performance of the M4 Pro chip with active cooling.
*   **Best Loop Score:** 8180
*   **Lowest Loop Score:** 8076
*   **Stability:** **98.73%**
*   **Summary:** Excellent thermal management; the system maintains near-peak performance throughout the duration of the test.

![Plugged In | High Power Mode | Default Fan Curve](<截屏2026-04-30 13.03.45.png>)

---

### 2. Plugged In | High Power Mode | Fans Disabled
This test evaluates the hardware's passive cooling limits and the aggressiveness of the macOS thermal throttling algorithm.
*   **Best Loop Score:** 8178
*   **Lowest Loop Score:** 5038
*   **Stability:** **61.6%**
*   **Performance Curve:**
    *   **0–300s:** Scores declined steadily in a near-linear fashion as heat accumulated.
    *   **300s+:** Performance plateaued, maintaining a flat horizontal line once the thermal equilibrium/throttling floor was reached.
*   **Summary:** Significant throttling occurs without active cooling, losing approximately 38% of peak performance to protect hardware integrity.

![Plugged In | High Power Mode | Fans Disabled](<截屏2026-04-30 13.03.54.png>)

---

### 3. Battery Power | Low Power Mode | Fans Disabled
This configuration tests the efficiency and "sweet spot" of the M4 Pro silicon when power draw is intentionally capped.
*   **Best Loop Score:** 5755
*   **Lowest Loop Score:** 5600
*   **Stability:** **97.31%**
*   **Summary:** While the ceiling is lower, the system achieves remarkable stability. The heat output in Low Power Mode is low enough that the system remains stable even without fans.

![Battery Power | Low Power Mode | Fans Disabled](<截屏2026-04-30 13.04.02.png>)

## 📊 Intuitive Comparision

| Mode | Fans | Stability | Best Score | Lowest Score
| :--- | :--- | :--- | :--- | :---
| High Power (Plugged) | Default | 98.73% | 8180 | 8076
| High Power (Plugged) | Disabled | 61.6% | 8178 | 5038
| Low Power (Battery) | Disabled | 97.31% | 5755 | 5600

---

## 📈 Key Findings
*   **Active Cooling is Essential for Pro Workloads:** The 37% drop in stability when fans are disabled (High Power) highlights that the M4 Pro's 20-core GPU generates substantial heat that exceeds passive dissipation capabilities.
*   **Linear Throttling:** The M4 Pro exhibits a predictable, linear performance decay under thermal stress before hitting a hard power floor.
*   **Low Power Mode Efficiency:** In Low Power Mode, the device provides ~70% of the maximum GPU performance with nearly perfect stability and zero fan noise, making it ideal for quiet environments.