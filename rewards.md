---
layout: default
title: Rewards Catalog
body_class: page-rewards
---

<div class="container">
  <header class="page-header">
    <h1 class="page-title">Rewards Catalog</h1>
    <p class="page-subtitle">Redeem your points for amazing rewards</p>
  </header>

  <div class="filter-bar card">
    <div class="filter-bar__search">
      <input type="search" class="form-input" id="rewards-search" placeholder="Search rewards..." />
    </div>
    <div class="filter-bar__categories" id="filter-categories">
      <button class="filter-pill filter-pill--active" data-filter="all">All</button>
      <button class="filter-pill" data-filter="gift-cards">Gift Cards</button>
      <button class="filter-pill" data-filter="travel">Travel</button>
      <button class="filter-pill" data-filter="merchandise">Merchandise</button>
      <button class="filter-pill" data-filter="experiences">Experiences</button>
      <button class="filter-pill" data-filter="charity">Charity</button>
    </div>
    <div class="filter-bar__sort">
      <select class="form-input form-input--sm" id="rewards-sort">
        <option value="featured">Featured</option>
        <option value="points-asc">Points: Low to High</option>
        <option value="points-desc">Points: High to Low</option>
        <option value="popular">Most Popular</option>
      </select>
    </div>
  </div>

  <div class="points-banner card" id="points-banner" style="display:none;">
    <span class="points-banner__label">Your balance:</span>
    <span class="points-banner__value" id="catalog-balance">--</span>
    <span class="points-banner__icon">pts</span>
    <a href="/jekyll-rewards-site/dashboard/" class="btn btn--ghost btn--sm">Dashboard</a>
  </div>

  <div class="rewards-grid" id="rewards-grid">
    <div class="skeleton-card card"></div>
    <div class="skeleton-card card"></div>
    <div class="skeleton-card card"></div>
    <div class="skeleton-card card"></div>
    <div class="skeleton-card card"></div>
    <div class="skeleton-card card"></div>
  </div>

  <div id="rewards-empty" class="empty-state" style="display:none;">
    <span class="empty-state__icon">search</span>
    <h3>No rewards found</h3>
    <p>Try adjusting your search or filter.</p>
    <button class="btn btn--ghost" onclick="document.getElementById('rewards-search').value=''; window.renderRewards();">Clear search</button>
  </div>
</div>
