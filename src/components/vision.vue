<template>
    <section class="mission-vision">
      <div class="content-wrapper">
        <div class="card-container">
          <article class="mission-card">
            <img loading="lazy" src="https://cdn.builder.io/api/v1/image/assets/TEMP/d93f35e4166a6e79a39e399b5d15a1b211bbb62e6874328e282d9c5ee0583281?placeholderIfAbsent=true&apiKey=5acb37f697474270ad553272da64e56a" class="card-image" alt="Mission illustration" />
            <h2 class="card-title">Our Mission</h2>
            <p class="card-description">
              At SelvyTex, we strive to be a global leader in exceptional quality, client trust, and employee well-being, driving innovation and sustainability for a brighter, greener future.
            </p>
          </article>
          <article class="vision-card">
            <img loading="lazy" src="https://cdn.builder.io/api/v1/image/assets/TEMP/00c5b319b2044c444bc9b73d17a589842e0989194a0697dbd7ea8411a77dced0?placeholderIfAbsent=true&apiKey=5acb37f697474270ad553272da64e56a" class="card-image" alt="Vision illustration" />
            <h2 class="card-title">Our Vision</h2>
            <p class="card-description">
              At <span class="highlight">SelvyTex</span>, we strive to be a global leader in exceptional quality, client trust, and employee well-being, driving innovation and sustainability for a brighter, greener future.
            </p>
          </article>
        </div>
      </div>
    </section>
  </template>
  
  <style scoped>
  .mission-vision {
    padding-top: 89px;
    margin-top: 8em;
  }
  
  .content-wrapper {
    background-color: rgba(224, 112, 64, 0.47);
    display: flex;
    align-items: center;
    padding: 0 12em 97px;
  }
  
  .card-container {
    z-index: 10;
    margin-top: -89px;
    width: 100%;
    max-width: 1103px;
    display: flex;
    gap: 20px;
  }
  
  .mission-card,
  .vision-card {
    border-radius: 15px;
    background-color: #fff;
    box-shadow: 14px 14px 14px rgba(0, 0, 0, 0.25);
    border-top: 10px solid #e07040;
    display: flex;
    flex-grow: 1;
    flex-direction: column;
    overflow: hidden;
    align-items: center;
    text-transform: uppercase;
    width: 50%;
    padding: 45px 40px 85px;
  }
  
  .card-image {
    aspect-ratio: 1;
    object-fit: contain;
    object-position: center;
    width: 176px;
    max-width: 100%;
  }
  
  .card-title {
    color: #e07040;
    letter-spacing: 2px;
    margin-top: 25px;
    font: 600 40px/1 Magra, sans-serif;
  }
  
  .card-description {
    color: rgba(0, 0, 0, 0.7);
    text-align: center;
    align-self: stretch;
    margin-top: 25px;
    font: 400 15px/27px Outfit, sans-serif;
  }
  
  .highlight {
    font-weight: 700;
    font-size: 20px;
    color: #e07040;
  }
  
  @media (max-width: 991px) {
    .content-wrapper {
      max-width: 100%;
      padding: 0 20px;
    }
  
    .card-container {
      max-width: 100%;
      flex-direction: column;
      align-items: stretch;
      gap: 40px;
    }
  
    .mission-card,
    .vision-card {
      max-width: 100%;
      width: 100%;
      padding: 45px 20px 85px;
    }
  
    .card-title {
      margin-top: 40px;
    }
  }
  </style>