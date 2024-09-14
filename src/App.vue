<script setup></script>

<template>
  <div class="d-grid">
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=10" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=11" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=12" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=13" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=14" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=15" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=15" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=15" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=15" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=15" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
    <div class="item">
      <img src="https://picsum.photos/300/200/?random=15" />
      <div>
        <p class="text">Lorem ipsum dolor sit amet.</p>
      </div>
    </div>
  </div>

  <div>add func1</div>
  <div>add func2</div>
  <div>add func3</div>
</template>

<style>
body {
  background: #302e36;
}
</style>

<style scoped>
.d-grid {
  padding: 20px;
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  /* column-gap: 12px; */
  /* row-gap: 12px; */
  gap: 12px;
  /* grid-template-columns: 200px 200px 200px 200px; */
  grid-template-columns: repeat(4, 1fr);
}

@media screen and (max-width: 972px) {
  .d-grid {
    padding: 8px;
    grid-template-columns: repeat(3, 1fr);
  }
}

@media screen and (max-width: 576px) {
  .d-grid {
    padding: 8px;
    grid-template-columns: repeat(2, 1fr);
  }
}

.item {
  /* height: 200px; */
  border: 1px solid #fff;
  background: #67607a;
  border-radius: 8px;
  box-shadow:
    0 0px 4px 2px rgba(255, 255, 255, 0.15),
    0 0px 4px 2px rgba(255, 255, 255, 0.15);
  display: flex;
  flex-flow: column;
  align-items: center;
  padding: 20px;
  gap: 12px;
}

/* item > src內有picsum */
.item > img[src*='picsum'] {
  width: 100px;
  aspect-ratio: 1/1;
  object-fit: cover;
}
</style>
