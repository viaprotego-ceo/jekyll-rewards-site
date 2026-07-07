---
layout: default
title: Welcome
body_class: page-home
---

<section class="hero">
  <div class="container hero-inner">
    <div class="hero-text">
      <span class="hero-badge">Loyalty Rewards Program</span>
      <h1 class="hero-title">Earn Points. Unlock Rewards.</h1>
      <p class="hero-subtitle">Join thousands of members earning points on every interaction. Redeem for gift cards, products, travel, and more.</p>
      <div class="hero-actions">
        <a href="{{ '/login/' | relative_url }}" class="btn btn--primary btn--lg">Get Started Free</a>
        <a href="{{ '/rewards/' | relative_url }}" class="btn btn--ghost btn--lg">Browse Rewards</a>
      </div>
    </div>
    <div class="hero-visual">
      <div class="hero-card card">
        <div class="hero-card__top">
          <span class="hero-card__label">Member Since 2024</span>
          <span class="hero-card__tier tier-gold">Gold</span>
        </div>
        <div class="hero-card__points">
          <span class="hero-points-value">12,450</span>
          <span class="hero-points-label">Points Available</span>
        </div>
        <div class="hero-card__progress">
          <div class="progress-bar">
            <div class="progress-bar__fill" style="width: 62%"></div>
          </div>
          <p class="progress-label">7,550 pts to Platinum status</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="features">
  <div class="container">
    <h2 class="section-title text-center">How It Works</h2>
    <div class="features-grid">
      <div class="feature-card card">
        <div class="feature-icon">shop</div>
        <h3>Earn Points</h3>
        <p>Earn points on purchases, referrals, reviews, and daily check-ins. Every action counts.</p>
      </div>
      <div class="feature-card card">
        <div class="feature-icon">chart</div>
        <h3>Level Up</h3>
        <p>Reach Silver, Gold, and Platinum tiers for bonus multipliers and exclusive member perks.</p>
      </div>
      <div class="feature-card card">
        <div class="feature-icon">gift</div>
        <h3>Redeem Rewards</h3>
        <p>Choose from hundreds of gift cards, travel, merchandise, and charitable donations.</p>
      </div>
    </div>
  </div>
</section>

<section class="cta-section">
  <div class="container text-center">
    <h2>Ready to start earning?</h2>
    <p>Sign in or create your account to begin your rewards journey.</p>
    <a href="{{ '/login/' | relative_url }}" class="btn btn--primary btn--lg">Sign In to Your Account</a>
  </div>
</section>
