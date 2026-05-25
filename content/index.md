---
title: "الصفحة الرئيسية"
---

<!-- 1. Media query layer isolated safely at the top -->
<style>
  .cards-container {
    display: flex;
    flex-direction: column;
    gap: 16px;
    width: 100%;
    margin-top: 24px;
    direction: rtl;
  }
  .custom-card {
    display: block;
    padding: 20px;
    border: 1px solid var(--lightgray);
    border-radius: 8px;
    text-align: center;
    text-decoration: none;
    font-weight: bold;
    background: var(--light);
    color: var(--dark);
    width: 100%;
    box-sizing: border-box;
  }
  @media (min-width: 600px) {
    .cards-container {
      flex-direction: row-reverse;
      flex-wrap: wrap;
    }
    .custom-card {
      width: calc(50% - 8px);
    }
  }
</style>

<!-- 2. Clean semantic HTML free of inline conflicting layout rules -->
<div class="cards-container">
  <a href="/regular-lessons" class="custom-card">الدروس المنتظمة</a>
  <a href="/special-lessons" class="custom-card">الدروس الخاصة</a>
  <a href="/summaries" class="custom-card">ملخصات عامة</a>
</div>



---

## 02


<div style="display: flex; flex-direction: column; gap: 16px; margin-top: 24px; direction: rtl;">
  <!-- Desktop Media Query Override Class using native styling fallback -->
  <style>
    @media (min-width: 600px) {
      .cards-container { flex-direction: row-reverse !important; flex-wrap: wrap; }
      .custom-card { width: calc(50% - 12px) !important; }
    }
  </style>
  
  <div class="cards-container" style="display: flex; flex-direction: column; gap: 16px; width: 100%;">
    
<a href="/regular-lessons" class="custom-card" style="display: block; padding: 20px; border: 1px solid var(--lightgray); border-radius: 8px; text-align: center; text-decoration: none; font-weight: bold; background: var(--light); color: var(--dark);">
    الدروس المنتظمة
</a>

<a href="/special-lessons" class="custom-card" style="display: block; padding: 20px; border: 1px solid var(--lightgray); border-radius: 8px; text-align: center; text-decoration: none; font-weight: bold; background: var(--light); color: var(--dark);">
    الدروس الخاصة
</a>

<a href="/summaries" class="custom-card" style="display: block; padding: 20px; border: 1px solid var(--lightgray); border-radius: 8px; text-align: center; text-decoration: none; font-weight: bold; background: var(--light); color: var(--dark);">
    ملخصات عامة
</a>


  </div>
</div>



---
## Hey




<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin-top: 20px;">

<a href="/regular-lessons" style="border: 1px solid var(--lightgray); padding: 20px; border-radius: 8px; text-align: center; text-decoration: none; font-weight: bold;">
الدروس المنتظمة
</a>

<a href="/special-lessons" style="border: 1px solid var(--lightgray); padding: 20px; border-radius: 8px; text-align: center; text-decoration: none; font-weight: bold;">
الدروس الخاصة
</a>

<a href="/summaries" style="border: 1px solid var(--lightgray); padding: 20px; border-radius: 8px; text-align: center; text-decoration: none; font-weight: bold;">
ملخصات عامة
</a>


</div>