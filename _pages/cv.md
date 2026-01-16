---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Sudharsun Lakshmi Narasimhan  
📍 Hyderabad, India  
📧 sudhas1728@gmail.com  
📞 +91 7538896597  

Incoming **Senior Engineer – Platform Security @ Qualcomm**  
Interests: Confidential Computing, Kernel Security, Network Security, Remote Attestation, Secure Systems

---

## Education

**Erasmus Mundus Joint Master’s Degree (Honors) in Security and Cloud Computing**  
Aalto University, Finland & EURECOM, France  
*Aug 2023 – Sep 2025*  
CGPA: **4.74 / 5**

**B.Tech in Computer Science and Engineering**  
Amrita School of Engineering, India  
*Jun 2016 – Jun 2020*  
CGPA: **8.68 / 10**

---

## Experience

### Security System Engineer — Ericsson HQ  
*Dec 2025 – Present*  
- Assessing risks and security posture of RAN compute and cloud infrastructure.

### Master’s Thesis Researcher — Ericsson Nomadic Lab (Publication)  
*Kista, Sweden | Mar 2025 – Sep 2025*  
- Kernel-based Remote Attestation framework using eBPF system call tracing, TLS 1.3 packet analysis, Measured Boot, and TPM.  
- Loadable Kernel Module (LKM) using kfuncs, crypto APIs, character devices.  
- Extended kernel-generated signing keys into TPM PCRs.  
- Built a Temporal Convolutional Neural Network (TCN) for anomaly detection in syscall sequences.

### Security Research Trainee — Ericsson Nomadic Lab  
*Kirkkonummi, Finland | May 2024 – Aug 2024*  
- Built Elastic QUIC Reverse Proxy inside Intel SGX enclave (EGo, Golang, Attested TLS, Azure Attestation).  
- Automated performance analysis using Python.

### Teaching Assistant — Aalto University  
*Espoo, Finland | Jan 2024 – Feb 2024*  
- Evaluated and graded platform security exercises.  
- Provided structured feedback to improve student comprehension.

### Network Consulting Engineer — Cisco Systems  
*Bengaluru, India | Jan 2020 – Aug 2023*  
- Built a web application for 5G Packet Core automation.  
- Worked on Kubernetes-based containerized network functions.  
- Automated network configuration and monitoring with Python.  
- Mentored junior engineers.

---

## Technical Skills

**Areas of Interest:**  
Confidential Computing, Network Security, Software Development  

**Languages & Frameworks:**  
C, C++, Python, React, Django, SQL, MongoDB  

**Tools & Technologies:**  
Remote Attestation, eBPF, 5G Networks, Wireshark, Git, Containers  

---

## Academic Projects

### eBPF-Based Memory Dump Tool  
*Co-developed with Andrea Oliveri | Oct 2024 – Feb 2025*  
- Built an eBPF-based memory forensics tool for RAM capture and analysis.  
- Worked on kernel internals, uprobes, and memory management.

---

## Publications

<ul>
{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

---

## Talks

<ul>
{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}
</ul>

---

## Teaching

<ul>
{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
</ul>

---

## Awards

- Ericsson Cooperation and Collaboration Award — *June 2025*  
- Aalto School of Science, Dean’s Incentive Scholarship — *Nov 2024*  
- Erasmus Mundus Joint Master Degree (EMJMD) Scholarship — *Aug 2023*  
- Cisco Connected Recognition Award — *Mar 2022*

---
