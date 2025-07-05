<template>
  <div class="landing-page">
    <header class="hero">
      <h1 class="name">철학과 예술을 사랑하는 사람</h1>
      <p class="subtitle">문학 • 음악 • 철학의 세계를 탐험합니다</p>
    </header>

    <main class="content">
      <section class="interests">
        <div class="interest-card">
          <h2>🤔 철학</h2>
          <p>이마누엘 칸트의 사상을 통해<br>인간 이성의 한계와 가능성을 탐구합니다</p>
        </div>

        <div class="interest-card">
          <h2>🎵 음악</h2>
          <p>모차르트의 음악에서<br>완벽한 조화와 아름다움을 발견합니다</p>
        </div>

        <div class="interest-card">
          <h2>📚 문학</h2>
          <p>도스토예프스키의 작품을 통해<br>인간 영혼의 깊이를 들여다봅니다</p>
        </div>
      </section>

      <footer class="quote">
        <p>"사는 것이 고통스럽더라도, 살아야 한다"</p>
        <span>- 도스토예프스키</span>
      </footer>
    </main>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Georgia', serif;
  line-height: 1.6;
}

.landing-page {
  min-height: 100vh;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 2rem;
}

.hero {
  text-align: center;
  margin-bottom: 4rem;
}

.name {
  font-size: 3rem;
  margin-bottom: 1rem;
  font-weight: 300;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.subtitle {
  font-size: 1.3rem;
  opacity: 0.9;
  font-style: italic;
}

.interests {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  max-width: 1200px;
  margin: 0 auto 4rem;
}

.interest-card {
  background: rgba(255, 255, 255, 0.1);
  padding: 2rem;
  border-radius: 15px;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  text-align: center;
  transition: transform 0.3s ease;
}

.interest-card:hover {
  transform: translateY(-5px);
}

.interest-card h2 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.interest-card p {
  font-size: 1.1rem;
  line-height: 1.6;
}

.quote {
  text-align: center;
  max-width: 600px;
  margin: 0 auto;
  padding: 2rem;
  background: rgba(255, 255, 255, 0.05);
  border-radius: 10px;
  border-left: 4px solid #ffd700;
}

.quote p {
  font-size: 1.4rem;
  font-style: italic;
  margin-bottom: 0.5rem;
}

.quote span {
  font-size: 1rem;
  opacity: 0.8;
}

@media (max-width: 768px) {
  .name {
    font-size: 2rem;
  }
  
  .subtitle {
    font-size: 1.1rem;
  }
  
  .interests {
    grid-template-columns: 1fr;
  }
}
</style>