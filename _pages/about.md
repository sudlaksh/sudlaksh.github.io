---
permalink: /
author_profile: true
redirect_from:
- /about/
- /about.html
---
<!-- Name - CENTERED, left-to-right line reveal -->
<div id="intro" class="name-center">
  <p class="line">Hey, I’m <strong>Sudharsun Lakshmi Narasimhan</strong> 👋</p>
</div>

<!-- Bio - LEFT-aligned, left-to-right word reveal -->
<div id="bio-reveal">
  <p class="bio-line" data-text="I am an incoming Senior Engineer - Platform Security at Qualcomm, Hyderabad, with experience in trusted computing, kernel security, and network automation."></p>
  <p class="bio-line" data-text="I hold an Erasmus Mundus Joint Master's degree in Security and Cloud Computing, as part of which I completed studies at Aalto University, Finland, and EURECOM, France. My academic and research work spans confidential computing, remote attestation, eBPF-based monitoring, and secure 5G systems. I have contributed to research at Ericsson Nomadic Lab, Finland, focusing on kernel-level attestation, system call tracing, QUIC protocol, and SGX-based secure networking."></p>
  <p class="bio-line" data-text="Prior to my master's, I worked at Cisco, where I contributed to automation and full-stack development for large-scale 5G packet core deployments using Kubernetes and containerized systems. My foundation in computer science began during my undergraduate studies at Amrita School of Engineering, Coimbatore, where I developed a strong interest in systems and security."></p>
  <p class="bio-line" data-text="I am particularly interested in platform security and network security, and I enjoy exploring practical applications of Artificial Intelligence in cybersecurity. I am always open to learning, collaboration, and contributing to meaningful security research and engineering efforts."></p>
</div>
{% raw %}
<script>
// Name reveal (CENTERED position, left→right animation)
const nameLines = document.querySelectorAll('#intro .line');
let nameIndex = 0;

function revealNameNext() {
  if (nameIndex < nameLines.length) {
    nameLines[nameIndex++].classList.add('visible');
  }
}

const nameInterval = setInterval(() => {
  if (nameIndex >= nameLines.length) {
    clearInterval(nameInterval);
    setTimeout(startBioReveal, 1200);
  } else {
    revealNameNext();
  }
}, 1000);

// Bio reveal (LEFT-aligned, left→right word-by-word)
const bioLines = document.querySelectorAll('.bio-line');
let currentBioLine = 0;
let currentBioWord = 0;

bioLines.forEach(line => line.innerHTML = '');

function revealBioNextWord() {
  if (currentBioLine >= bioLines.length) return;
  
  const line = bioLines[currentBioLine];
  const fullText = line.getAttribute('data-text');
  const words = fullText.split(' ');
  
  if (currentBioWord < words.length) {
    const wordSpan = document.createElement('span');
    wordSpan.textContent = words[currentBioWord] + ' ';
    wordSpan.classList.add('bio-word');
    line.appendChild(wordSpan);
    currentBioWord++;
    setTimeout(revealBioNextWord, 50);
  } else {
    currentBioLine++;
    currentBioWord = 0;
    setTimeout(revealBioNextWord, 300);
  }
}

function startBioReveal() {
  revealBioNextWord();
}

// Single interaction reveals everything instantly
['click', 'keydown', 'wheel', 'touchstart'].forEach(event =>
  window.addEventListener(event, () => {
    // Reveal name
    nameLines.forEach(line => line.classList.add('visible'));
    // Reveal bio
    bioLines.forEach(line => {
      line.innerHTML = line.getAttribute('data-text') + ' ';
      line.classList.add('revealed');
    });
  }, { once: true })
);
</script>
{% endraw %}
