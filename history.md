---
layout: default
title: Transaction History
body_class: page-history
---

<div class="container" id="history-root">

  <div id="history-auth-gate" class="auth-gate" style="display:none;">
    <div class="auth-gate__inner card">
      <span class="auth-gate__icon">lock</span>
      <h2>Sign in to view your transaction history</h2>
      <a href="/jekyll-rewards-site/login/" class="btn btn--primary btn--lg">Sign In</a>
    </div>
  </div>

  <div id="history-content" style="display:none;">
    <header class="page-header">
      <h1 class="page-title">Transaction History</h1>
      <p class="page-subtitle">All your points activity in one place</p>
    </header>

    <div class="history-summary">
      <div class="summary-card card">
        <p class="summary-value summary-value--earn" id="hist-total-earned">--</p>
        <p class="summary-label">Total Earned</p>
      </div>
      <div class="summary-card card">
        <p class="summary-value summary-value--redeem" id="hist-total-spent">--</p>
        <p class="summary-label">Total Redeemed</p>
      </div>
      <div class="summary-card card">
        <p class="summary-value" id="hist-balance">--</p>
        <p class="summary-label">Current Balance</p>
      </div>
    </div>

    <div class="filter-bar card">
      <div class="filter-bar__search">
        <input type="search" class="form-input" id="history-search" placeholder="Search transactions..." />
      </div>
      <div class="filter-bar__categories">
        <button class="filter-pill filter-pill--active" data-filter="all">All</button>
        <button class="filter-pill" data-filter="earn">Earned</button>
        <button class="filter-pill" data-filter="redeem">Redeemed</button>
        <button class="filter-pill" data-filter="bonus">Bonuses</button>
      </div>
      <div class="filter-bar__sort">
        <select class="form-input form-input--sm" id="history-sort">
          <option value="newest">Newest First</option>
          <option value="oldest">Oldest First</option>
          <option value="points-desc">Most Points</option>
          <option value="points-asc">Fewest Points</option>
        </select>
      </div>
    </div>

    <div class="transaction-list card" id="history-list">
      <p class="loading-text">Loading transactions...</p>
    </div>

    <div id="history-empty" class="empty-state" style="display:none;">
      <span class="empty-state__icon">inbox</span>
      <h3>No transactions found</h3>
      <p>Your points activity will appear here once you start earning.</p>
    </div>

    <div class="pagination" id="history-pagination"></div>
  </div>
</div>
