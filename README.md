# Wireshark Network Traffic Analysis

## 📌 Objective
To capture live network traffic using Wireshark, filter specific protocols, and analyze packet behavior for educational or troubleshooting purposes.

---

## 🛠️ Tools Used
- **Wireshark** (latest version)
- **Operating System**: Windows / macOS / Linux
- **Browser**: Chrome / Firefox / Edge

---

## 🔄 Procedure

1. Open **Wireshark**.
2. Select the active network interface (**Wi-Fi or Ethernet**) to begin capturing.
3. Click the **Start** button to begin live packet capture.
4. Open a web browser and visit a website (e.g., `https://example.com`) to generate traffic.
5. After about 1 minute, return to Wireshark and click the **Stop** button.
6. Apply a filter in the display filter bar (e.g., `http`, `dns`, `tcp`) to focus on specific protocols.
7. Note: **Filter keywords must be written in lowercase** (e.g., `http`, not `HTTP`).
8. Export the filtered packets via **File > Export Specified Packets** and select **Displayed** to save only the filtered results as a `.pcap` file.

---

## 📦 Files Included

- `http.pcap` — Sample filtered packet capture showing HTTP traffic
- `Wireshark_Report.docx` — Summary report of findings and analysis

---

## 🔍 Protocols Observed

| Protocol | Description                        |
|----------|------------------------------------|
| DNS      | Domain Name System queries         |
| TCP      | Transmission Control Protocol      |
| HTTP     | Hypertext Transfer Protocol (web)  |

---

## 📈 Key Observations

- Total packets captured: 51,506  
- Filtered packets using `http`: 459  
- Observed traffic from DNS resolution to HTTP request-response cycle
- TCP was used for reliable communication

---

## ✅ Conclusion

Wireshark successfully captured live traffic. By applying protocol filters (using lowercase keywords), we could isolate and analyze specific types of packets like HTTP, DNS, and TCP. This provides hands-on insight into how data moves across a network.

---

## 📌 Notes

- Filters in Wireshark are **case-sensitive** — always use **lowercase protocol names**.
- Make sure to select **"Displayed"** when exporting to only save filtered packets.

---

