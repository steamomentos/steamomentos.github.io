# STEAMomentos: رسوم تفاعلية

رسوم تفاعلية تحل محل الصور الثابتة في مقالات [steamomentos.org](https://steamomentos.org). كل رسم ملف HTML مستقل (CSS و JS داخليان)، عربي RTL، يتبع هوية STEAMomentos البصرية وشروط كتاب *Explaining Research*.

التنظيم: `<قسم الموقع>/<رابط المقالة>/<الرسم>.html`

رابط التضمين: `https://steamomentos.github.io/<المسار>`

```html
<iframe src="https://steamomentos.github.io/<المسار>" style="width:100%;border:0;min-height:640px" loading="lazy" title="..."></iframe>
<!-- اختياري، مرة واحدة في الصفحة: يجعل ارتفاع الإطار يطابق المحتوى تلقائيًا -->
<script>
addEventListener('message', e => {
  if (e.data && e.data.type === 'sm-embed-height')
    document.querySelectorAll('iframe').forEach(f => { if (f.contentWindow === e.source) f.style.height = e.data.height + 'px'; });
});
</script>
```

## المقالات

### الكيمياء: [المحفزات في إنتاج وتخزين الهيدروجين](https://steamomentos.org/articles/almhfzat-fy-antag-otkhzyn-alhydrogyn)
| الشكل | الملف |
|---|---|
| (1) أنواع المحفزات | [`fig1-catalyst-types.html`](chemistry/almhfzat-fy-antag-otkhzyn-alhydrogyn/fig1-catalyst-types.html) |
| (2) تحلل الأمونيا بالحفز | [`fig2-ammonia-decomposition.html`](chemistry/almhfzat-fy-antag-otkhzyn-alhydrogyn/fig2-ammonia-decomposition.html) |
| (3) تشكيل الأطر المعدنية العضوية | [`fig3-mof-assembly.html`](chemistry/almhfzat-fy-antag-otkhzyn-alhydrogyn/fig3-mof-assembly.html) |
| (4) التقاط CO₂ وتحويله | [`fig4-co2-capture-conversion.html`](chemistry/almhfzat-fy-antag-otkhzyn-alhydrogyn/fig4-co2-capture-conversion.html) |
| (5) تخزين الطاقة المتجددة | [`fig5-renewable-energy-storage.html`](chemistry/almhfzat-fy-antag-otkhzyn-alhydrogyn/fig5-renewable-energy-storage.html) |
