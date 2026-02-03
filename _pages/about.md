---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<div id="intro">

  <p class="line">
    Hey, I’m <strong>Sudharsun Lakshmi Narasimhan</strong> 👋 — an incoming <strong>Senior Engineer – Platform Security</strong> at <strong>Qualcomm, Hyderabad</strong>, working at the intersection of <strong>trusted computing</strong>, <strong>kernel systems</strong>, and <strong>secure networking</strong>. My work spans both <strong>industry and research</strong>, from building kernel-level attestation frameworks and eBPF monitoring tools to exploring <strong>secure 5G systems</strong> and <strong>confidential computing</strong> in cloud-native environments. Previously, I contributed to <strong>5G network automation at Cisco</strong> and conducted research at <strong>Ericsson Nomadic Lab</strong>, focusing on remote attestation, SGX-based secure networking, and system call anomaly detection. I hold an <strong>Erasmus Mundus Master’s in Security & Cloud Computing</strong>, studied at <strong>Aalto University 🇫🇮</strong> and <strong>EURECOM 🇫🇷</strong>, and began my journey in computer science at <strong>Amrita School of Engineering, India</strong>. Beyond systems and security, I enjoy <strong>building practical security solutions</strong>, experimenting with <strong>AI in cybersecurity</strong>, and collaborating on <strong>meaningful research projects</strong>.
  </p>

</div>

{% raw %}
<script>
  const lines = document.querySelectorAll('.line');
  let index = 0;
  let revealedAll = false;

  function revealNext() {
    if (index < lines.length) {
      lines[index++].classList.add('visible');
    }
  }

  function revealAll() {
    if (revealedAll) return;
    revealedAll = true;
    lines.forEach(line => line.classList.add('visible'));
  }

  const interval = setInterval(() => {
    if (index >= lines.length) {
      clearInterval(interval);
    } else {
      revealNext();
    }
  }, 800);

  ['click', 'keydown', 'wheel', 'touchstart'].forEach(event =>
    window.addEventListener(event, revealAll, { once: true })
  );
</script>
{% endraw %}
