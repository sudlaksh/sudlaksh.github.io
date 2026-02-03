---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<div id="intro">

<p class="line">Hey, I’m <strong>Sudharsun Lakshmi Narasimhan</strong> 👋</p>

<p class="line spacer">
<strong>Incoming Senior Engineer – Platform Security</strong><br>
at <strong>Qualcomm, Hyderabad</strong>, working at the intersection of<br>
<strong>trusted computing</strong>, <strong>kernel systems</strong>,<br>
and <strong>secure networking</strong>.
</p>

<p class="line">
My work spans <strong>industry and research</strong>:<br>
<strong>kernel attestation frameworks</strong>, <strong>eBPF monitoring tools</strong>,<br>
<strong>secure 5G systems</strong>, <strong>confidential computing</strong>.
</p>

<p class="line">
<strong>Cisco:</strong> 5G network automation.<br>
<strong>Ericsson Nomadic Lab:</strong> remote attestation, SGX networking,<br>
system call anomaly detection.
</p>

<p class="line">
<strong>Erasmus Mundus Master’s</strong> – <strong>Security & Cloud Computing</strong>,<br>
<strong>Aalto University 🇫🇮</strong>, <strong>EURECOM 🇫🇷</strong>,<br>
<strong>Amrita School of Engineering, India</strong>.
</p>

<p class="line">
I enjoy building <strong>practical security solutions</strong>,<br>
<strong>AI in cybersecurity</strong>, and collaborating on<br>
<strong>meaningful research projects</strong>.
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
