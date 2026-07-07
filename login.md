---
layout: default
title: Sign In
body_class: page-login
hide_nav: true
---

<div class="auth-container">
  <div class="auth-card card">
    <div class="auth-logo">
      <span class="auth-logo__icon">*</span>
      <span class="auth-logo__text">RewardHub</span>
    </div>
    <h1 class="auth-title">Welcome back</h1>
    <p class="auth-subtitle">Sign in to view your points and rewards</p>

    <div id="auth-error" class="alert alert--error" style="display:none;"></div>

    <form class="auth-form" id="login-form" novalidate>
      <div class="form-group">
        <label class="form-label" for="email">Email address</label>
        <input class="form-input" type="email" id="email" name="email" placeholder="you@example.com" autocomplete="email" required />
        <span class="form-error" id="email-error"></span>
      </div>

      <div class="form-group">
        <label class="form-label" for="password">
          Password
          <a href="/forgot-password/" class="form-label__link">Forgot password?</a>
        </label>
        <div class="input-with-toggle">
          <input class="form-input" type="password" id="password" name="password" placeholder="........" autocomplete="current-password" required />
          <button type="button" class="input-toggle" id="password-toggle" aria-label="Show password">show</button>
        </div>
        <span class="form-error" id="password-error"></span>
      </div>

      <div class="form-group form-group--row">
        <label class="form-checkbox">
          <input type="checkbox" id="remember-me" name="remember" />
          <span>Remember me for 30 days</span>
        </label>
      </div>

      <button type="submit" class="btn btn--primary btn--full btn--lg" id="login-submit">
        <span id="login-btn-text">Sign In</span>
        <span id="login-btn-spinner" class="spinner" style="display:none;"></span>
      </button>
    </form>

    <div class="auth-divider"><span>Demo credentials</span></div>
    <div class="demo-credentials">
      <p>Use any of these to explore:</p>
      <div class="demo-users">
        <button class="demo-user-btn" data-email="alice@example.com" data-pass="demo1234">
          <strong>Alice Johnson</strong> - Gold member
        </button>
        <button class="demo-user-btn" data-email="bob@example.com" data-pass="demo1234">
          <strong>Bob Smith</strong> - Silver member
        </button>
        <button class="demo-user-btn" data-email="carol@example.com" data-pass="demo1234">
          <strong>Carol Davis</strong> - Platinum member
        </button>
      </div>
    </div>
  </div>
</div>
