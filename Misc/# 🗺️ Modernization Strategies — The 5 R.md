# 🗺️ Modernization Strategies — The 5 R's

> 🎯 This guide is for trainers to explain the industry-standard cloud migration strategies
> and show where GitHub Copilot App Modernization fits in.

When organizations plan a cloud journey, they evaluate every legacy application against
one of five standard strategies — known as the **"5 R's of Cloud Migration"**
(popularized by Gartner and AWS). Understanding these helps you explain *why* not all
apps are modernized the same way, and exactly where GitHub Copilot App Modernization
delivers the most value.

---

## 📊 The 5 R's at a Glance

| Strategy | Also Known As | Modernization Level | Effort | Long-Term Value |
| -------- | ------------- | ------------------- | ------ | --------------- |
| ⬆️ Rehosting | Lift and Shift | 🔴 Low | Low | Low |
| 🏗️ Replatforming | Lift and Reshape | 🟡 Medium | Medium | Medium–High |
| 🧩 Refactoring | Rearchitecting | 🟢 High | High | Highest |
| 🛒 Repurchasing | Drop and Shop | N/A | Medium | Medium |
| 🛑 Retiring | Decommission | N/A | Low | Immediate savings |

---

## 1. ⬆️ Rehosting — "Lift and Shift"

**What it is:** Move the exact same application and its operating system from an
on-premise server directly to a Cloud VM — without changing any code or architecture.

**Real-world example:** Taking a Java 8 app running on a Windows Server VM in your
data center and moving it to an Azure VM running the same Windows Server image.

**Pros:**
- ✅ Fastest path out of the data center
- ✅ Lowest upfront cost and risk
- ✅ No code changes required

**Cons:**
- ❌ All technical debt moves with you to the cloud
- ❌ No access to cloud-native features (auto-scaling, managed services)
- ❌ Still paying for always-on VMs — no cost optimization
- ❌ Still vulnerable to the same CVEs and EOL issues

> 🚫 **The key limitation:** You get a new address, not a new house.

---

## 2. 🏗️ Replatforming — "Lift and Reshape" or "Lift and Optimize"

**What it is:** Move to the cloud, but make *targeted improvements* to take advantage
of cloud capabilities — without rewriting the core business logic.

**Real-world examples