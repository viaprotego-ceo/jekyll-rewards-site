---
layout: default
title: Dashboard
body_class: page-dashboard
---

<div class="container dashboard" id="dashboard-root">

  <div id="auth-gate" class="auth-gate" style="display:none;">
    <div class="auth-gate__inner card">
      <span class="auth-gate__icon">lock</span>
      <h2>Sign in to view your dashboard</h2>
      <p>Access your points balance, tier status, and recent activity.</p>
      <a href="/jekyll-rewards-site/login/" class="btn btn--primary btn--lg">Sign In</a>
    </div>
  </div>

  <div id="dashboard-content" style="display:none;">
    <header class="dashboard-header">
      <div>
        <h1 class="dashboard-title">Hello, <span id="dash-first-name">--</span>!</h1>
        <p class="dashboard-subtitle">Here is your rewards summary</p>
      </div>
      <div class="dashboard-tier">
        <span class="tier-badge" id="dash-tier-badge">--</span>
      </div>
    </header>

    <div class="kpi-grid">
      <div class="kpi-card card">
        <div class="kpi-icon">pts</div>
        <div class="kpi-body">
          <p class="kpi-value" id="dash-points">--</p>
          <p class="kpi-label">Points Balance</p>
        </div>
      </div>
      <div class="kpi-card card">
        <div class="kpi-icon">gift</div>
        <div class="kpi-body">
          <p class="kpi-value" id="dash-redeemed">--</p>
          <p class="kpi-label">Rewards Redeemed</p>
        </div>
      </div>
      <div class="kpi-card card">
        <div class="kpi-icon">fire</div>
        <div class="kpi-body">
          <p class="kpi-value" id="dash-streak">--</p>
          <p class="kpi-label">Day Streak</p>
        </div>
      </div>
      <div class="kpi-card card">
        <div class="kpi-icon">cal</div>
        <div class="kpi-body">
          <p class="kpi-value" id="dash-this-month">--</p>
          <p class="kpi-label">Earned This Month</p>
        </div>
      </div>
    </div>

    <div class="tier-progress-card card">
      <div class="tier-progress-header">
        <h2>Tier Progress</h2>
        <span id="dash-tier-label">--</span>
      </div>
      <div class="progress-bar progress-bar--lg">
        <div class="progress-bar__fill" id="dash-tier-progress" style="width:0%"></div>
      </div>
      <p class="progress-label" id="dash-tier-next">--</p>
    </div>

    <div class="quick-actions">
      <h2 class="section-title">Quick Actions</h2>
      <div class="quick-actions-grid">
        <a href="/jekyll-rewards-site/rewards/" class="quick-action-btn card">
          <span class="quick-action-icon">gift</span>
          <span>Browse Rewards</span>
        </a>
        <button class="quick-action-btn card" id="checkin-btn">
          <span class="quick-action-icon">check</span>
          <span>Daily Check-In</span>
        </button>
        <a href="/jekyll-rewards-site/history/" class="quick-action-btn card">
          <span class="quick-action-icon">list</span>
          <span>View History</span>
        </a>
        <a href="/jekyll-rewards-site/profile/" class="quick-action-btn card">
          <span class="quick-action-icon">user</span>
          <span>My Profile</span>
        </a>
      </div>
    </div>

    <div class="recent-activity">
      <div class="section-header">
        <h2 class="section-title">Recent Activity</h2>
        <a href="/jekyll-rewards-site/history/" class="btn btn--ghost btn--sm">View all</a>
      </div>
      <div class="activity-list card" id="dash-activity-list">
        <p class="loading-text">Loading activity...</p>
      </div>
    </div>

    <div class="featured-rewards">
      <div class="section-header">
        <h2 class="section-title">Featured Rewards</h2>
        <a href="/jekyll-rewards-site/rewards/" class="btn btn--ghost btn--sm">View all</a>
      </div>
      <div class="rewards-grid" id="dash-featured-rewards">
        <p class="loading-text">Loading rewards...</p>
      </div>
    </div>
  </div>
</div>
