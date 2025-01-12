<div style="display: flex; justify-content: center; align-items: center; gap: 20px;">
  <div align="left" style="flex: 1;">
    <div id="text-gif" style="font-size: 24px; font-family: Arial, sans-serif; color: #ffffff;"></div>
  </div>
  <div align="right" style="flex: 1;">
    <img src="https://66.media.tumblr.com/43ff1ae84968ffd84606207e9995a78e/tumblr_py4mvbGe6h1tgo74ho1_1280.gif" height="250" width="200" alt="cyberpunk gif">
  </div>
</div>

<script>
  const textGifElement = document.getElementById("text-gif");
  const text = "Hi, welcome to my GitHub";
  let index = 0;
  let isDeleting = false;

  function animateText() {
    if (!textGifElement) return;

    if (!isDeleting) {
      textGifElement.textContent = text.substring(0, index);
      index++;
      if (index > text.length) {
        isDeleting = true;
        setTimeout(animateText, 1000); // Pause before deleting
        return;
      }
    } else {
      textGifElement.textContent = text.substring(0, index);
      index--;
      if (index < 0) {
        isDeleting = false;
        setTimeout(animateText, 500); // Pause before typing again
        return;
      }
    }

    setTimeout(animateText, isDeleting ? 50 : 100); // Speed adjustment
  }

  animateText();
</script>

## Techs
<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" height="40" alt="c logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" height="40" alt="java logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" height="40" alt="vscode logo"  />
</div>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/JMischa/JMischa/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/JMischa/JMischa/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/JMischa/JMischa/output/github-snake.svg" />
</picture>
