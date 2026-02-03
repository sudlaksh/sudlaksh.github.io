---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<div id="intro">

  <p class="line">Hey, welcome 👋</p>

  <p class="line">
    I’m <strong>Sudharsun Lakshmi Narasimhan</strong>.
  </p>

  <p class="line spacer">
    I work at the intersection of<br>
    <strong>platform security</strong>, <strong>kernel systems</strong>,<br>
    and <strong>secure networking</strong>.
  </p>

  <p class="line">
    I’m an <strong>incoming Senior Engineer – Platform Security</strong><br>
    at <strong>Qualcomm, Hyderabad</strong>.
  </p>

  <p class="line">
    My work spans <strong>industry and academic research</strong>,<br>
    with a focus on <strong>trusted computing</strong> and
    <strong>cloud-native systems</strong>.
  </p>

  <p class="line">
    I hold an <strong>Erasmus Mundus Joint Master’s</strong><br>
    in <strong>Security & Cloud Computing</strong>,<br>
    completed at <strong>Aalto University 🇫🇮</strong> and
    <strong>EURECOM 🇫🇷</strong>.
  </p>

  <p class="line">
    My interests include <strong>confidential computing</strong>,<br>
    <strong>remote attestation</strong>, <strong>eBPF-based monitoring</strong>,<br>
    and <strong>secure 5G systems</strong>.
  </p>

  <p class="line">
    I enjoy building <strong>practical security systems</strong>,<br>
    exploring <strong>AI in cybersecurity</strong>,<br>
    and collaborating on <strong>meaningful research</strong>.
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
  }, 1500);

  ['click', 'keydown', 'wheel', 'touchstart'].forEach(event =>
    window.addEventListener(event, revealAll, { once: true })
  );
</script>
{% endraw %}
