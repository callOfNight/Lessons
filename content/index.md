---
title: "الصفحة الرئيسية"
---


<style>
  .lessons-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 16px;
    width: 100%;
    margin-top: 28px;
    direction: rtl;
  }
  
  .lesson-btn {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 22px 28px;
    background: var(--light);
    border: 1px solid var(--lightgray);
    border-radius: 12px;
    text-decoration: none;
    font-size: 1.25rem;
    font-weight: 700;
    color: var(--dark);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
    transition: all 0.2s ease-in-out;
  }

  .lesson-btn::after {
    content: "←";
    font-size: 1.4rem;
    color: var(--secondary);
    transition: transform 0.2s ease;
  }

  /* Desktop and Tablet optimization */
  @media (min-width: 768px) {
    .lessons-grid {
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }
    .lesson-btn:hover {
      transform: translateY(-3px);
      border-color: var(--secondary);
      box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
    }
    .lesson-btn:hover::after {
      transform: translateX(-5px);
    }
  }
</style>

<div class="lessons-grid">
  <a href="/regular-lessons" class="lesson-btn">الدروس المنتظمة</a>
  <a href="/special-lessons" class="lesson-btn">الدروس الخاصة</a>
  <a href="/summaries" class="lesson-btn">ملخصات عامة</a>
</div>